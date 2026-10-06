# GrokDay for Windows Terminal

Windows Terminal color scheme for [GrokDay](https://github.com/xai-org/grok-build/blob/main/crates/codegen/xai-grok-pager-render/src/theme/grokday.rs), the light theme used by Grok Build.

Each slot uses a color token from that file. The hex values are unchanged.

| Slot | Token | Hex |
|---|---|---|
| background | bg_base | `#EEEEEE` |
| foreground, black, brightWhite | text_primary | `#262626` |
| cursorColor, white | text_secondary / accent_user | `#444444` |
| selectionBackground | bg_visual | `#C6C6C6` |
| brightBlack | gray_bright | `#626262` |
| red / brightRed | RED / RED1 | `#CD3048` / `#AF2323` |
| green / brightGreen | GREEN / GREEN1 | `#378E23` / `#0C947C` |
| yellow / brightYellow | YELLOW / accent_plan | `#A27612` / `#A8780A` |
| blue / brightBlue | BLUE / BLUE0 | `#2F64D2` / `#28448A` |
| purple / brightPurple | MAGENTA / PURPLE | `#7D4BC6` / `#6C3EB2` |
| cyan / brightCyan | CYAN / TEAL | `#0082AA` / `#0A8E70` |

Path orange `#C3691E`, verify violet `#7850A0`, remember green `#4CAF50`, and the pale diff backgrounds have no ANSI slot. Grok still paints those itself.

## Install

1. In Windows Terminal, open the settings JSON with Ctrl+, then the settings button, or open `%LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState\settings.json`.
2. Copy the object in [`grokday.json`](grokday.json) into the `schemes` array.
3. Set the profile default:

```json
"profiles": {
    "defaults": {
        "colorScheme": "GrokDay"
    }
}
```

Open a new tab to see it.

The palette comes from xai-org/grok-build and is under the Apache License 2.0. See `NOTICE`.
