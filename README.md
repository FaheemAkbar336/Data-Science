# Pakistan Laws Legal Assistant

A smart AI assistant that analyzes legal text and delivers accurate, easy-to-understand guidance. Built to reduce research time and improve legal workflow efficiency.

## Project Structure

```
project/
├── backend/                    # Backend Python application
│   ├── backend-main.py        # Main backend server
│   ├── backend_model.py       # AI model integration
│   ├── analysis_module.py     # Legal analysis module
│   ├── document_parser.py     # Document parsing utilities
│   ├── laws-retriever.py      # Laws retrieval system
│   ├── prompt.py              # AI prompt templates
│   ├── requirements.txt       # Python dependencies
│   ├── pakistan_laws_dataset.csv
│   └── pdf_data.json
├── frontend/                   # Frontend web application
│   ├── frontend-index.html    # Main HTML file
│   ├── frontend-app.js        # JavaScript application logic
│   └── frontend-style.css     # Styling
└── data/                       # Data files
    └── pak_constitution/
        ├── constitution.json
        └── constitution.csv
```

## Features

- Legal document analysis
- Pakistan Constitution search and retrieval
- AI-powered legal assistance
- Web-based user interface
- Real-time legal text parsing and interpretation

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Modern web browser (Chrome, Firefox, Safari, Edge)
- OpenAI API key

## Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/FaheemAkbar336/Data-Science.git
cd project

# 2. Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Linux/Mac
# .venv\Scripts\activate  # On Windows

# 3. Install dependencies
cd backend
pip install -r requirements.txt

# 4. Configure environment variables
# Create a .env file and add your OpenAI API key:
# OPENAI_API_KEY=your-api-key-here

# 5. Start the backend server
python backend-main.py

# 6. Open frontend in your browser
# Open frontend/frontend-index.html or serve with a web server
```

## Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/FaheemAkbar336/Data-Science.git
cd project
```

### Step 2: Set up Virtual Environment
```bash
python -m venv .venv
source .venv/bin/activate  # On Linux/Mac
# .venv\Scripts\activate  # On Windows
```

### Step 3: Install Backend Dependencies
```bash
cd backend
pip install -r requirements.txt
```

### Step 4: Configure Environment Variables
1. Create a `.env` file in the `backend` directory:
```
OPENAI_API_KEY=your-openai-api-key-here
```

2. Get your OpenAI API key from [https://platform.openai.com/api-keys](https://platform.openai.com/api-keys)

### Step 5: Run the Application
```bash
# Terminal 1: Start the backend server
cd backend
python backend-main.py
```

Then open `frontend/frontend-index.html` in your web browser or serve it using a local web server:
```bash
# Terminal 2: Serve frontend (optional, for better functionality)
cd frontend
python -m http.server 8000
# Then visit http://localhost:8000/frontend-index.html
```

## Usage

1. **Start the backend server**:
   ```bash
   cd backend
   python backend-main.py
   ```

2. **Open the frontend**:
   - Open `frontend/frontend-index.html` in your web browser
   - Or serve it using a local web server

3. **Use the assistant**:
   - Enter your legal query or upload a document
   - The AI will analyze and provide guidance
   - Review the results and references

## Dependencies

### Backend
- **Flask** - Web framework for API
- **openai** - OpenAI API integration for AI-powered analysis
- **python-docx** - Word document processing
- **PyPDF2** - PDF document processing
- **python-dotenv** - Environment variable management

### Frontend
- HTML5
- CSS3
- Vanilla JavaScript

## Configuration

### Environment Variables
Create a `.env` file in the `backend` directory:
```
OPENAI_API_KEY=your_api_key_here
FLASK_ENV=development
FLASK_DEBUG=True
```

### API Keys
- **OpenAI API Key**: Required for legal analysis. Get it from [OpenAI Platform](https://platform.openai.com/api-keys)

## Troubleshooting

**Issue**: Module not found error
- **Solution**: Ensure virtual environment is activated and all dependencies are installed
  ```bash
  pip install -r requirements.txt
  ```

**Issue**: OPENAI_API_KEY not found
- **Solution**: Check that `.env` file exists in the `backend` directory with the correct key

**Issue**: Port already in use
- **Solution**: Change the port in `backend-main.py` or kill the process using the port

**Issue**: Frontend not loading
- **Solution**: Ensure backend server is running on `http://localhost:5000` (or configured port)

## Project Status

- **Status**: Active Development (Beta)
- **Last Updated**: April 2026

## Roadmap

- [ ] Multi-language support (Urdu, English)
- [ ] PDF upload and analysis improvements
- [ ] Case law database integration
- [ ] User authentication and history
- [ ] Mobile app version
- [ ] Advanced search filters

## API Endpoints (Backend)

- `POST /analyze` - Analyze legal text
- `GET /search?query=` - Search laws database
- `POST /upload` - Upload and process documents

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

- **Author**: Faheem Akbar
- **GitHub**: [@FaheemAkbar336](https://github.com/FaheemAkbar336)
- **Email**: Contact via GitHub profile

## Disclaimer

This application is designed to provide legal information and assistance. It is not a substitute for professional legal advice. Always consult with a qualified legal professional for specific legal matters.

---

**Last Updated**: April 2026
**Version**: 1.0.0-beta
