# Cangjie Practice Tool

<div align="center">
   
   ![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/ikwbb/cangjie-practice-tool)
   
   <img src="demo/demo.gif" alt="Demo of the Cangjie Practice Tool">


   [Try it out online!](https://ikwbb.github.io/cangjietraining/)

</div><br>

A web-based tool designed to help users practice and learn the Cangjie input method, a popular Chinese character input system. This project supports both traditional and simplified Chinese characters, with customizable difficulty levels based on character frequency.

## Features

- **Interactive Practice**: Type Cangjie codes to match displayed Chinese characters.
- **Difficulty Settings**: Choose character frequency ranges (1-7072) to adjust practice difficulty.
- **Simplified/Traditional Toggle**: Switch between simplified and traditional Chinese characters.
- **Answer Display**: Show Cangjie codes and graphical breakdowns (for traditional characters) with a button or Enter key.
- **Progress Navigation**: Go back to the previous character using a button or Shift + Backspace.
- **Mobile-Friendly**: Responsive design with adjustments for mobile devices.
- **Local Storage**: Saves your difficulty and character set preferences.


## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/cangjie-practice.git
   ```
2. **Navigate to the Project Directory**:
   ```bash
   cd cangjie-practice
   ```
3. **Open in Browser**:
   Simply open `index.html` in a web browser. No server setup is required as it runs entirely client-side.

   Alternatively, use a local server for better performance:
   ```bash
   npx http-server
   ```
   Then visit `http://localhost:8080` in your browser.

## Usage

1. **Select Difficulty**: 
   - Check the boxes in the "Settings and Help" panel to choose character frequency ranges (e.g., 1-500 for beginners, up to 7001-7072 for advanced).
   - At least one range must be selected.

2. **Choose Character Set**: 
   - Toggle the "Use Simplified Characters" checkbox to switch between traditional (default) and simplified Chinese.

3. **Practice**: 
   - A Chinese character appears in the center.
   - Type its Cangjie code in the input box. Correct input advances to the next character automatically.
   - Press `Enter` or click "Ans" to reveal the code and (for traditional characters) a graphical breakdown.

4. **Navigation**: 
   - Click the `<` button or press `Shift + Backspace` to return to the previous character.

5. **Tips**: 
   - Click the `···` button to open the settings and help panel.

## Project Structure

```
cangjie-practice/
├── index.html         # Main HTML file
├── style.css          # Styling for the interface
├── script.js          # Core logic and event handling
├── cangjie5.js        # Cangjie code mappings
├── cangjieToKeyboard.js # Conversion utilities
└── README.md          # Project documentation
```

## Dependencies

- No external libraries are required; the project uses vanilla JavaScript and HTML/CSS.
- Data sources:
  - [HKCards Cangjie Dictionary](https://www.hkcards.com/)
  - [CUHK Common Character Frequency Table](https://humanum.arts.cuhk.edu.hk/Lexis/lexi-can/faq.php?s=1)
  - [GitHub: staristic/BIG5-JSON](https://github.com/staristic/BIG5-JSON)
  - [GitHub: cheukyin699/cangjie-dictionary](https://github.com/cheukyin699/cangjie-dictionary)

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m "Add feature"`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a pull request.

Please ensure your code follows the existing style and includes appropriate comments.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
