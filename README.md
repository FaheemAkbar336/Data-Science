# Pakistan Laws Legal Assistant

A web-based legal assistant application that provides analysis and information about Pakistan's laws and constitution.

## Project Structure

```
project/
├── backend/                    # Backend Python application
│   ├── backend-main.py        # Main backend server
│   ├── backend_model.py       # AI model integration
│   ├── analysis_module.py     # Legal analysis module
│   ├── document_praser.py     # Document parsing utilities
│   ├── laws-retriever.py      # Laws retrieval system
│   ├── prompt.py              # AI prompt templates
│   ├── requirements.txt       # Python dependencies
│   ├── pakistan_laws_dataset.csv
│   └── pdf_data.json
├── frontend/                   # Frontend web application
│   ├── Frontened-index.html   # Main HTML file
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

## Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Modern web browser

## Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd project
```

2. Create a virtual environment (recommended):
```bash
python -m venv .venv
.venv\Scripts\activate  # On Windows
```

3. Install backend dependencies:
```bash
cd backend
pip install -r requirements.txt
```

4. Set up environment variables:
   - Create a `.env` file in the backend directory
   - Add your OpenAI API key: `OPENAI_API_KEY=your-api-key-here`

## Usage

1. Start the backend server:
```bash
cd backend
python backend-main.py
```

2. Open the frontend:
   - Open `frontend/Frontened-index.html` in your web browser
   - Or serve it using a local web server

## Dependencies

### Backend
- Flask - Web framework
- openai - OpenAI API integration
- python-docx - Word document processing
- PyPDF2 - PDF document processing

## Configuration

Make sure to configure your API keys and environment variables before running the application.

## License

[Add your license information here]

## Contributing

[Add contribution guidelines here]

## Contact

[Add your contact information here]
