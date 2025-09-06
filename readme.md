# Locale & Keyboard Layout Test

This project is a small web app that helps you test how your **system locale** and **keyboard layout** are detected in the browser.  

It displays:  
- **Locale information**: browser language, time zone, date formatting, currency formatting.  
- **Interactive keyboard diagram**: visualizes a keyboard layout (US, UK, DE, FR, ES included).  
- **Key logging**: highlights pressed keys and shows their `KeyboardEvent.code` and `KeyboardEvent.key`.  
- **Auto-detection**: tries to guess your keyboard layout based on certain key presses (for example `Shift+2`).  
- **Manual override**: switch layouts from a dropdown to compare.

## Usage

1. Clone or download this repository.  
2. Open `locale-keyboard-test.html` in any modern browser.  
3. The page will automatically show your locale and default to a US keyboard layout.  
4. Press some keys (especially `Shift+2` and `\`) to let the script guess your actual keyboard layout.  
5. Use the dropdown to manually switch between layouts if needed.

## Features

- Works fully client-side (no backend required).  
- Highlights pressed keys in real-time.  
- Logs key events for debugging.  
- Includes 5 layouts out of the box:
  - 🇺🇸 en-US  
  - 🇬🇧 en-GB  
  - 🇩🇪 de-DE  
  - 🇫🇷 fr-FR  
  - 🇪🇸 es-ES  

(Additional layouts such as IT, NL, SE, NO, JP can be added.)

## Example

When running with a UK region but a US keyboard:
- Dates and currency will format in UK style (DD/MM/YYYY, £).  
- Pressing `Shift+2` will log `@` (US layout), even though locale is `en-GB`.  

This helps spot mismatches between system locale and physical keyboard layout.

## License

MIT
