# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Single self-contained static HTML/CSS file, no build step (user's choice). Hostable on GitHub Pages later.

## Users

Two audiences, weighted equally:

- **Video editors on DaVinci Resolve Free** who want to drive Resolve by talking to an AI assistant instead of clicking through menus, and who don't want to pay $295 for Studio. Technical enough to follow a four-step install (copy a script, create a Python venv, edit an MCP config).
- **Developers and AI-tool users** already running Cursor, Claude Desktop, Windsurf or another MCP client, looking to add Resolve to their setup. They look for the mechanism, tool coverage, install commands and config snippets.

## Product Purpose

davinci-resolve-mcp is an MCP server that lets AI assistants control DaVinci Resolve through natural language ("Add a marker at 5 seconds", "Transcribe my timeline", "Render to MP4"). Success: a visitor understands that it works on the free version of Resolve, trusts the mechanism, and gets it running.

## Positioning

The only DaVinci Resolve MCP server that works on the **Free** version. Other Resolve MCP servers rely on external scripting, which Blackmagic restricts to the paid Studio version. This project instead runs a small bridge script *inside* Resolve via Workspace → Scripts (available to everyone), which opens a localhost connection the MCP server talks to.

## Operating Context

- Architecture: AI assistant → (MCP) → `resolve_mcp_bridge.py` on the user's machine → (HTTP, localhost) → `CursorBridge.py` running inside Resolve → DaVinci Resolve API (read + write).
- Requirements: DaVinci Resolve 18+ (Free or Studio), Python 3.9+ on the same machine, an MCP-compatible assistant.
- Install: copy `src/CursorBridge.py` into the Resolve scripts folder (paths differ for Windows, macOS, Linux); clone, create venv, `pip install -r requirements.txt`; add the server to `.cursor/mcp.json` or equivalent (WSL variant exists); in Resolve run Workspace → Scripts → CursorBridge; console shows `Bridge is running (read + write)`.
- Part of a three-server pipeline with mcp-image-gen (local image generation) and a file-based Video Editor MCP (ffmpeg).

## Capabilities and Constraints

- 162 MCP tools across Timeline, Clips, Markers & Flags, Media Pool, Color Grading, Fusion, Rendering, Titles, Audio, Gallery, Tracks, Project Management, AI Tools.
- 155 of 162 tools work on Free. The rest are Studio Neural Engine features.
- Local AI replacements (no API keys, no cloud, CPU only, models download on first use): Voice Isolation via Demucs v4 (Meta); Background Removal via rembg + BiRefNet; Auto Subtitles via faster-whisper.
- No alternative on Free: Smart Reframe, Stabilization.
- Limitations: no keyframe animation (static values only); Fusion node parameters need the Fusion page UI; transitions must be added manually; background removal on video is CPU-bound and slow for long clips; gallery stills require the Color page.
- Counts: 7 tools need Studio's Neural Engine; 5 of those have local replacements (covering 3 features: voice isolation, background removal, subtitles); 2 have none (Smart Reframe, Stabilization). Per README.

## Brand Commitments

- Name: davinci-resolve-mcp ("DaVinci Resolve MCP Bridge").
- Creator: **hiteshK03 (Hitesh Kandala)**, MIT license. Upstream: https://github.com/hiteshK03/davinci-resolve-mcp. Every surface credits the creator and links upstream.
- This repository (Bridgepointglobal/Video-editing-) is an unmodified point-in-time copy. Surfaces carry no Bridgepoint branding and must not present themselves as an official site of the project or claim affiliation with Blackmagic Design.
- "DaVinci Resolve" is Blackmagic Design's product; refer to it by name only, never mimic its logo or UI branding.
- Voice: plain, direct, slightly playful README tone ("Just talk to your AI assistant. It controls Resolve for you.").

## Evidence on Hand

- README.md: example prompts, tool-area table, Free vs Studio table, install steps, limitations.
- `examples/mcp.json` config example.
- No screenshots, videos, logos, testimonials, user counts, stars or press. Do not fabricate any of these.

## Product Principles

1. Lead with the Free-version mechanism; it is the one claim nobody else can make.
2. Be honest about limits: name what doesn't work alongside what does.
3. Show the conversation: real example prompts are the clearest demonstration of value.
4. Credit the creator visibly; this is someone else's open-source work.
5. Get people running: install steps must be complete and copyable.
