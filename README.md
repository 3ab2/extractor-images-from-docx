# 🖼️ D-GITALCODE Word Image Extractor Pro

<div align="center">

[![Python 3.11+](https://img.shields.io/badge/Python-3.11%2B-3776ab?logo=python&logoColor=white)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![GitHub Release](https://img.shields.io/github/v/release/3ab2/extractor-images-from-docx?include_prereleases)](https://github.com/3ab2/extractor-images-from-docx/releases)

**Professional Image Extraction Tool for Word Documents**

*Extract, manage, and export images from DOCX/DOC files with advanced processing capabilities*

[📥 Install](#-installation) • [🚀 Quick Start](#-usage) • [✨ Features](#-features) • [📖 Documentation](#-project-structure)

</div>

---

## 📋 Overview

**D-GITALCODE Word Image Extractor Pro** is a powerful, enterprise-grade Python application designed to extract, analyze, and manage images from Word documents (DOCX/DOC). Built for developers, document processors, and businesses, this tool streamlines image extraction workflows with an intuitive GUI and advanced reporting capabilities.

Whether you're working with large document archives, automating document processing, or managing image assets, Word Image Extractor Pro delivers efficiency and precision.

---

## ✨ Features

- ✅ **Multi-Format Support** – Extract images from DOCX and DOC files seamlessly
- ✅ **Batch Processing** – Process multiple documents in a single operation
- ✅ **Format-Based Extraction** – Filter and extract images by format (PNG, JPG, BMP, etc.)
- ✅ **Duplicate Detection** – Automatically identify and remove duplicate images
- ✅ **Modern GUI** – Professional, responsive interface built with CustomTkinter
- ✅ **Real-Time Progress Tracking** – Monitor extraction progress with detailed status updates
- ✅ **Advanced Reporting** – Generate reports in TXT, PDF, and Excel formats
- ✅ **Theme Support** – Seamlessly switch between Dark and Light modes
- ✅ **Multi-Language** – Full support for English (EN), Français (FR), and العربية (AR)
- ✅ **Comprehensive Logging** – Detailed logs for debugging and audit trails
- ✅ **Organized Output** – Automatically structured extraction results

---

## 📸 Screenshots

> **Main Interface** – Clean, intuitive dashboard for document selection and extraction controls

> **Extraction Progress** – Real-time progress monitoring with detailed statistics

> **Report Generation** – Professional reports in multiple formats (TXT, PDF, Excel)

---

## 💾 Installation

### System Requirements

- **Python**: 3.11 or higher
- **OS**: Windows, macOS, or Linux
- **Memory**: Minimum 2 GB RAM
- **Disk Space**: 500 MB for dependencies and temporary files

### Step 1: Clone the Repository

```bash
git clone https://github.com/3ab2/extractor-images-from-docx.git
cd extractor-images-from-docx
```

### Step 2: Create a Virtual Environment (Recommended)

```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Dependencies

The following packages are automatically installed:

- **python-docx** – Word document parsing and manipulation
- **Pillow** – Image processing and format handling
- **CustomTkinter** – Modern GUI framework
- **openpyxl** – Excel report generation
- **reportlab** – PDF report generation
- **python-dotenv** – Environment configuration management

---

## 🚀 Usage

### Running the Application

```bash
python main.py
```

### Basic Workflow

1. **Launch the Application** – Start the GUI with the command above
2. **Select Documents** – Choose one or multiple Word documents from your file system
3. **Configure Settings** (Optional)
   - Choose output directory
   - Enable/disable duplicate detection
   - Select image formats to extract
   - Choose report format (TXT, PDF, Excel)
4. **Start Extraction** – Click the "Extract" button to begin processing
5. **Monitor Progress** – View real-time extraction status and statistics
6. **Review Results** – Access extracted images and generated reports in the output folder

### Command-Line Usage (Advanced)

```python
from extractor import ImageExtractor

extractor = ImageExtractor()
extractor.extract_from_docx('document.docx', output_dir='./images')
```

---

## 📁 Project Structure

```
D-GITALCODE-Word-Image-Extractor-Pro/
│
├── main.py                 # Application entry point
├── gui.py                  # GUI components and interface
├── extractor.py            # Core extraction logic
├── report.py               # Report generation utilities
├── utils.py                # Helper functions and utilities
├── config.py               # Configuration management
├── requirements.txt        # Python dependencies
├── LICENSE                 # MIT License
├── README.md               # This file
│
├── resources/
│   ├── icons/             # Application icons and assets
│   └── languages/         # Localization files (EN, FR, AR)
│
├── output/                # Default extraction output directory
└── logs/                  # Application logs
```

---

## 🛠️ Technologies & Stack

| Technology | Version | Purpose |
|-----------|---------|---------|
| **Python** | 3.11+ | Core language |
| **CustomTkinter** | Latest | GUI framework |
| **python-docx** | Latest | DOCX/DOC parsing |
| **Pillow** | Latest | Image processing |
| **openpyxl** | Latest | Excel export |
| **reportlab** | Latest | PDF generation |

---

## 🔧 Configuration

Edit the configuration settings in `config.py`:

```python
# Output directory for extracted images
OUTPUT_DIR = './extracted_images'

# Enable duplicate detection
DETECT_DUPLICATES = True

# Supported image formats
SUPPORTED_FORMATS = ['png', 'jpg', 'jpeg', 'bmp', 'gif', 'tiff']

# Report generation
GENERATE_REPORTS = True
REPORT_FORMATS = ['txt', 'pdf', 'xlsx']

# Language setting
DEFAULT_LANGUAGE = 'EN'  # EN, FR, AR

# Theme
DEFAULT_THEME = 'dark'  # dark, light
```

---

## 📊 Output & Reports

The application generates three types of reports:

### 1. Text Report (TXT)
Simple, readable format with extraction summary and statistics.

### 2. PDF Report
Professional PDF document with images, metadata, and detailed analysis.

### 3. Excel Report (XLSX)
Structured spreadsheet with sortable data for further analysis.

Each report includes:
- Total images extracted
- Image formats breakdown
- Duplicate count
- Extraction timestamp
- File sizes and metadata

---

## 🌐 Multi-Language Support

D-GITALCODE Word Image Extractor Pro supports three languages:

- **English (EN)** – Complete English interface
- **Français (FR)** – Interface complète en français
- **العربية (AR)** – الواجهة الكاملة باللغة العربية

Change language in the GUI settings or modify `DEFAULT_LANGUAGE` in `config.py`.

---

## 📝 Logging

All operations are logged in the `logs/` directory:

```
logs/
├── application.log        # General application logs
├── extraction.log         # Extraction-specific logs
└── errors.log            # Error and exception logs
```

Enable detailed logging by adjusting the log level in `config.py`.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

For commercial licensing or custom deployments, contact **D-GITALCODE**.

---

## 👨‍💼 Author

**ELKARCH ABDELHAMID**

Senior Developer & Founder of D-GITALCODE

- 🌐 [D-GITALCODE Official](https://d-gitalcodema.vercel.app/fr)
- 📧 Email: 3ab2uelkarch2006@gmail.com
- 💼 LinkedIn: [D-GITALCODE](https://www.linkedin.com/in/d-gitalcode-elkarch-abdelhamid-0604583bb?utm_source=share_via&utm_content=profile&utm_medium=member_ios)

---

## 📞 Support & Contact

For issues, feature requests, or support:

- 📋 **GitHub Issues**: [Report an Issue](https://github.com/3ab2/extractor-images-from-docx/issues)
- 💬 **Discussions**: [Join our Community](https://github.com/3ab2/extractor-images-from-docx/discussions)
- 📧 **Direct Support**: 3ab2uelkarch2006@gmail.com

---

## 🎁 Acknowledgments

Built with passion and precision using cutting-edge Python libraries and design principles.

---

<div align="center">

**Developed with ❤️ by D-GITALCODE**

*ELKARCH ABDELHAMID*

*Professional Document Processing Solutions*

© 2024 D-GITALCODE. All rights reserved.

</div>
