# Cheating Daddy - Linux Edition =)

AI assistant for interviews.

Original repo: https://github.com/sohzm/cheating-daddy

## Quick Start

```bash
chmod +x Cheating-Daddy-Linux-0.5.0-FINAL.AppImage
./Cheating-Daddy-Linux-0.5.0-FINAL.AppImage
```

Get API key at [Google AI Studio](https://aistudio.google.com/apikey)

## Requirements

- Linux with PulseAudio or PipeWire
- `pacat` utility (usually pre-installed)

```bash
# If missing:
# Arch
sudo pacman -S pipewire-pulse

# Ubuntu/Debian
sudo apt install pulseaudio-utils
```

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Ctrl + Enter` | Screenshot + AI response |
| `Ctrl + Arrow` | Move window |
| `Ctrl + M` | Click-through mode |
| `Ctrl + H` | Hide/show window |
| `Ctrl + Shift + E` | Emergency quit |

## Audio Modes (Settings)

- **Speaker Only** (default) - hears only interviewer
- **Mic Only** - hears only you
- **Both** - hears both

## Troubleshooting

**No audio?** Check default output:
```bash
pactl get-default-sink
```

**AppImage won't start?**
```bash
sudo apt install libfuse2  # Ubuntu/Debian
sudo pacman -S fuse2       # Arch
```