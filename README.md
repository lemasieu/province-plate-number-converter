# Province Plate Number Converter

A simple, interactive web tool that converts between Vietnamese province names and their corresponding license plate number prefixes. It supports both lookup directions: finding the plate numbers for a given province, or identifying the province from a plate number.

## 🚀 Live Demo

Check out the live demo: [https://www.sieu.io.vn/github/province-plate-number-converter](https://www.sieu.io.vn/github/province-plate-number-converter)

## ✨ Features

- **Lookup by Province** – Select a province to view its current name, old name(s) (if any), and the associated license plate number prefixes
- **Lookup by Plate Number** – Enter a plate number prefix (e.g., `85`) to identify the corresponding province and its old name (if applicable)
- **Toggle Between Modes** – Switch between "Theo tỉnh" (By province) and "Theo biển số" (By plate number) with a single click
- **Comprehensive Data** – Covers all Vietnamese provinces and their historical plate number changes
- **Real-Time Results** – Results update instantly as you select a province or type a plate number
- **Clean Interface** – Simple, user-friendly design with a clear layout
- **Responsive** – Works on desktop, tablet, and mobile devices

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- JSON (province and plate number data)

## 📁 Project Structure

```
province-plate-number-converter/
├── index.html                    # Main HTML file
├── style.css                     # Stylesheet
├── script.js                     # JavaScript logic for lookups
├── data.json                     # Province and plate number data
└── README.md                     # Project documentation
```

## 🔧 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/lemasieu/province-plate-number-converter.git
   ```
2. **Navigate to the project folder**
   ```bash
   cd province-plate-number-converter
   ```
   
3. **Run the application with a local server**

⚠️ Important: This project loads data from a JSON file, so you need to use a local development server instead of opening `index.html` directly in your browser to avoid CORS issues.

- **Using VS Code** – Install the "Live Server" extension, right-click on `index.html`, and select "Open with Live Server"
- **Using Python** – Run `python -m http.server` (Python 3) or `python -m SimpleHTTPServer` (Python 2) and open `http://localhost:8000`
- **Using Node.js** – Install `http-server` globally (`npm install -g http-server`) and run `http-server` in the project folder

## 📝 How It Works

The tool provides two lookup modes:

### Lookup by Province (Theo tỉnh)

1. Select a province from the dropdown menu
2. The tool displays:
   - **Current province name** (Tên tỉnh hiện tại)
   - **Old province name** (Tên tỉnh cũ), if the province has undergone a name change or merger
   - **License plate numbers** (Biển số xe) associated with that province

### Lookup by Plate Number (Theo biển số)

1. Enter a plate number prefix into the input field (e.g., `85`)
2. The tool identifies the corresponding province and displays:
   - **Current province name**
   - **Old province name** (if applicable)
   - **License plate numbers associated with that province**

**How the data is structured:**

The `data.json` file contains entries for each province, including:
- `Province` – The current province name
- `OldProvinces` – An array or string of old province names (if any)
- `Number` – An array or string of license plate number prefixes

The tool matches user input against both current and old province names to ensure accurate results.

## 🤝 Contributing

Contributions are welcome! Feel free to submit a Pull Request or open an Issue.
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License
This project is open-source and available under the MIT License.
