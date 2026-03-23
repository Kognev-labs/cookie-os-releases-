# Changelog

All notable changes to Cookie OS will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/).

## [1.0.0] - 2026-03-23

### Added
- AI agent chat with streaming responses and session management
- Full email system with @mail.cookieos.app addresses — send, receive, and manage email directly from the desktop
- HTML email rendering with dark theme support and sandboxed iframe display
- Agent intelligence skills: smart briefing, session context, preference learning, action authority, and proactive initiative
- Kanban task board (Mission Control) with agent integration and REST API
- Reminders and cron jobs with local-first SQLite persistence and gateway sync
- Agent memory system with full-text search (FTS5)
- File browser with folder creation, rename, export, and base64 read
- Skills store (Cookie Store) with 7 built-in skills and hot-reload support
- Settings panel for AI provider, model, personality, and wallpaper configuration
- Guided onboarding wizard with runtime detection and auto-install
- Auto-update with changelog modal and background download
- Auto-move-to-Applications prompt on macOS first launch
- Secure container runtime (Podman/Docker) with hardened security (cap-drop ALL, no-new-privileges)
- Production code signing with Developer ID (Apple) and Apple notarization
- Sentry error tracking with PII redaction

### Platforms
- macOS Apple Silicon (arm64) — signed and notarized
- macOS Intel (x64) — signed and notarized
- Windows (x64) — NSIS installer

### Fixed
- Boot splash error handling with retry and skip options for returning users
- Broken memory API routes in core skills
- Chat UI fixes and streaming improvements
- Live progress bar, rotating security facts, and friendly errors during onboarding
- Carriage return handling in progress output
- Correct binary name in container runtime error messages
- Automatic old image cleanup during container updates
- Tool-only agent responses no longer invisible in chat
- Panel content overflow resolved with proper CSS constraints
- Skills store font sizes increased for readability
- Internal skill context filtered from chat history
- sql.js WASM path resolution for packaged builds
- Model selection, installer UX, and settings crash loop
