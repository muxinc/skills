# Mux Skill

> **Experimental**: This skill is under active development and may change significantly. Use at your own discretion.

A skill that provides comprehensive documentation and examples for building video applications with [Mux](https://mux.com).

## What is this?

This is a skill package that can be installed into AI coding assistants (Claude Code, Cursor, Windsurf, etc.) to give them deep knowledge about Mux's video infrastructure platform. When enabled, your AI assistant can help you:

- Build video-on-demand and live streaming applications
- Integrate Mux Player into web and mobile apps
- Set up video uploads with progress tracking
- Configure analytics and monitoring with Mux Data
- Implement content security (signed URLs, DRM)
- Work with AI-powered video features (auto-chapters, summarization, moderation)

## What's included

```
skills/mux/
├── SKILL.md              # Skill definition and quick start guide
├── reference/            # 40+ reference docs covering core concepts
│   ├── mux-fundamentals.md
│   ├── api-authentication.md
│   ├── mux-player-overview.md
│   ├── live-streaming-getting-started.md
│   ├── webhooks.md
│   └── ...
└── examples/             # 20 practical implementation examples
    ├── quickstart-stream-video.md
    ├── direct-upload-with-webhooks.md
    ├── live-streaming-complete-setup.md
    ├── ai-video-workflows.md
    └── ...
```

### Reference documentation covers

- **Core concepts**: Organizations, environments, assets, playback IDs, API structure
- **Mux Player**: Setup, customization, advanced features (Chromecast, AirPlay, DVR)
- **Video upload**: URL ingestion, direct uploads, Mux Uploader components
- **Live streaming**: RTMP/SRT ingest, latency modes, simulcasting, live clipping
- **Mux Data**: Metrics, dashboards, custom dimensions, alerts
- **Player integrations**: Video.js, HLS.js, Shaka, ExoPlayer, AVPlayer
- **Framework guides**: Next.js, React Native, Sanity CMS, and more
- **Security**: Signed URLs, DRM, CSP configuration

### Examples include

- End-to-end video upload with webhook handling
- Live streaming setup with embedded captions
- Signed URL playback with JWT generation
- React Native stories app implementation
- AI video workflows (chapters, summarization, moderation)

## Installation

```bash
npx skills add muxinc/skills
```

This will install the Mux skill into your AI coding assistant.

## Usage

Once installed, your AI assistant will automatically use this knowledge when you ask about Mux-related topics:

- "How do I upload a video to Mux?"
- "Set up live streaming with low latency"
- "Add Mux Player to my React app"
- "Configure webhooks to track video status"
- "Generate signed playback URLs"

## Requirements

- A Mux account with API credentials
- An AI coding assistant with skills support (Claude Code, Cursor, Windsurf, etc.)

## License

MIT
