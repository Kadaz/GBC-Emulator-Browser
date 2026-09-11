# Retro Browser Emulator

A lightweight collection of classic console emulators designed to run directly in a web browser.

The main goal of this project is **PlayStation 5 browser compatibility**, while also keeping the emulator simple and lightweight enough to run on ordinary desktop browsers.

## Current Features

* Play directly in the browser
* PlayStation 5 browser support
* DualSense controller support
* Keyboard support on PC
* On-screen controls
* ROMs loaded from the local `roms` folder
* No installation required
* Simple static web structure
* Designed to work without external emulator cores or downloads

* Test It Here: 

## PlayStation 5 Controls

### Game Boy

| Controller         | Action    |
| ------------------ | --------- |
| D-Pad / Left Stick | Direction |
| X                  | A         |
| O                  | B         |
| OPTIONS            | Pause     |

The on-screen controls can also be used when playing through the browser.

## Performance

The emulator uses a lightweight frame-based approach.

Because browser performance on PlayStation 5 is different from desktop browsers, the emulator can process multiple emulation frames during a browser frame when necessary.

This helps improve gameplay speed on systems where the browser cannot maintain the same performance as a desktop computer.

The exact speed multiplier may vary depending on the console being emulated and the capabilities of the browser.

## Compatibility

The project is primarily tested with:

* PlayStation 5 Browser
* Safari-based browser environment
* Desktop Chrome and other modern browsers

Desktop browsers generally provide better performance, while PlayStation 5 performance may vary depending on the game and emulator.

## Project Structure

```text
/
├── index.html
└── roms/
    ├── index.json
    └── game.gb
```

The `roms/index.json` file is used to list available games.

## Development Philosophy

The project focuses on keeping the emulator as lightweight and self-contained as possible.

Rather than relying on large external frameworks, downloadable cores, or WASM dependencies, the goal is to adapt the emulator itself for browser compatibility.

Special attention is given to PlayStation 5 browser input handling, performance and controller responsiveness.

## Planned Systems

The project will gradually expand to other classic systems using the same general approach:

* Game Boy
* Game Boy Color
* Atari
* NES
* Game Boy Advance

Each system will be developed and tested separately, with priority given to PlayStation 5 browser compatibility.

## Disclaimer

This project is intended for experimentation, preservation and educational purposes.

Users are responsible for ensuring that they have the legal right to use any ROM files loaded into the emulator.
