# BASICdraw

Draw lines and export to BASIC LINE commands for vintage computer systems.

A web application that lets you draw lines on a canvas and export them as authentic BASIC LINE commands. Perfect for retro programming enthusiasts who want to create graphics for classic BASIC dialects without manually plotting coordinates on graph paper!

**🌐 [Live Demo](https://basiclinedraw.netlify.app/)**

## Features

- **Interactive Drawing**: Click on the canvas to draw points and connect them with lines
- **Multiple BASIC Dialects**: Supports syntax for various vintage BASIC implementations:
  - GW-BASIC / QBasic / QuickBASIC (default)
  - Atari ST BASIC
  - Sharp MZ-700/800 BASIC
  - MSX BASIC
  - Commodore 128 BASIC 7.0
  - Apple II HPLOT
  - Generic BASIC
- **Multiple Resolutions**: Choose from classic computer resolutions:
  - 256×192 (MSX)
  - 280×192 (Apple II HGR2)
  - 320×200 (CGA/C64/Atari)
  - 640×350 (EGA)
  - 640×400 (Atari ST)
  - 640×480 (VGA)
- **Color Support**: Full EGA/VGA 16-color palette (0-15) with automatic color mapping for each dialect
- **Image Overlay**: Load reference images as an onion-skin overlay to trace and convert to BASIC code
- **Line Segments**: Create disconnected line segments using the "New Segment" button
- **Undo Functionality**: Remove the last drawn line with the "Undo" button
- **Customizable Line Numbers**: Set the starting line number for exported code
- **One-Click Copy**: Easily copy generated BASIC code to clipboard

## How to Use

1. **Select Your BASIC Dialect**: Choose the target BASIC dialect from the dropdown menu (defaults to GW-BASIC)
2. **Choose Resolution**: Select the appropriate resolution for your target system (automatically filtered based on dialect)
3. **Select Color**: Pick a color from the EGA/VGA palette (0-15) for your drawing
4. **(Optional) Load Image Overlay**: Click "📷 Load Image" to load a reference image as an overlay. Adjust opacity with the slider to trace over it
5. **Draw Lines**: Click on the canvas to place points. Consecutive clicks will be connected with lines
6. **Create Segments**: Click "New Segment" to start a disconnected line (useful for drawing separate shapes)
7. **Undo Mistakes**: Use the "Undo" button to remove the last drawn line
8. **Export Code**: Click "Export BASIC Code" to generate the LINE commands
9. **Copy**: Use the copy button to copy the generated code to your clipboard
10. **Clear**: Start over with the "Clear Canvas" button (overlay image is preserved)

## Example

Here's an example of creating a drawing with BASICdraw. First, the tool interface showing the drawing canvas with controls:

![BASICdraw Tool Interface](example-tool.png)

After drawing and exporting, the generated GW-BASIC code appears in the output area and can be imported to your BASIC interpreter. 

![BASICdraw Output](example-output.png)

The complete GW-BASIC code exported by the tool produces this output in BASIC.

## Technical Details

- **Pure HTML/CSS/JavaScript** - no dependencies required
- **Client-side only** - runs entirely in the browser, no server needed
- **Canvas-based drawing** with coordinate scaling and grid overlay
- **Image overlay support** - accepts common image formats (PNG, JPG, GIF, etc.), auto-scales to canvas width while maintaining aspect ratio
- **Automatic resolution filtering** based on selected BASIC dialect
- **Color mapping** - EGA/VGA colors automatically mapped to dialect-specific palettes (e.g., Apple II hi-res colors)
- **Optimized exports** - Apple II HPLOT only outputs `HCOLOR=` when color changes

## License

See [LICENSE](LICENSE) file for details.

## Credits
Made by [1XN.org](https://1xn.org) | [GitHub: 1xn](https://github.com/1xn)
