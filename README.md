# prvis-ai — LiveKit

Stripped LiveKit server for prvis-ai voice pipeline.

## What was removed
deploy scripts, test suite, build tools, magefiles, install scripts

## What was added
`prvis/livekit.yaml` — prvis server config with SIP enabled
`prvis/docker-compose.yml` — 512M RAM limit, agent-network

## Resource requirements
512M RAM, 0.5 CPU
Ports: 7880 (HTTP), 7881 (RTC TCP), 7882 (RTC UDP), 5060 (SIP)

## Used by
prvis voice agent — Moonshine STT + CosyVoice TTS + SpeechBrain voice auth
