# BASICdraw
Draw lines and export to BASIC LINE commands

A little web application that lets you draw lines on a canvas and export them as authentic BASIC LINE commands for vintage computer systems. Perfect for retro programming enthusiasts who want to create graphics for classic BASIC dialects without manually plotting coordinates on graph paper!

## Features

- **Interactive Drawing**: Click on the canvas to draw points and connect them with lines
- **Multiple BASIC Dialects**: Supports syntax for various vintage BASIC implementations:
  - Generic BASIC
  - Atari ST BASIC
  - GW-BASIC / QBasic / QuickBASIC
  - Sharp MZ-700/800 BASIC
  - MSX BASIC
  - Commodore 128 BASIC 7.0
- **Multiple Resolutions**: Choose from classic computer resolutions:
  - 256×192 (MSX)
  - 320×200 (CGA/C64/Atari)
  - 640×350 (EGA)
  - 640×400 (Atari ST)
  - 640×480 (VGA)
- **Line Segments**: Create disconnected line segments using the "New Segment" button
- **Customizable Line Numbers**: Set the starting line number for exported code
- **One-Click Copy**: Easily copy generated BASIC code to clipboard

## How to Use

1. **Select Your BASIC Dialect**: Choose the target BASIC dialect from the dropdown menu
2. **Choose Resolution**: Select the appropriate resolution for your target system
3. **Draw Lines**: Click on the canvas to place points. Consecutive clicks will be connected with lines
4. **Create Segments**: Click "New Segment" to start a disconnected line (useful for drawing separate shapes)
5. **Export Code**: Click "Export BASIC Code" to generate the LINE commands
6. **Copy**: Use the copy button to copy the generated code to your clipboard
7. **Clear**: Start over with the "Clear Canvas" button

## Example Output

For GW-BASIC with a line drawn from (100, 50) to (200, 150), the output would be:

```
10 LINE (100,50)-(200,150)
```

## Technical Details

- Pure HTML/CSS/JavaScript - no dependencies required
- Runs entirely in the browser
- Canvas-based drawing with coordinate scaling
- Automatic resolution filtering based on selected BASIC dialect

## License

See [LICENSE](LICENSE) file for details.

## Credits

Made by [1XN.org](https://1xn.org) | [GitHub: 1xn](https://github.com/1xn)
