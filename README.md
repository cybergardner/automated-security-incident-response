# Automated Security Incident Response System

This project demonstrates an automated system to ingest, detect, and respond to security incidents in real-time.

## Features
- Ingest logs via a Flask API.
- Parse and store security logs in JSON format.
- Future: Threat detection and automated incident response.

## Development Environment Setup

### Prerequisites
- Python 3.9+
- `pip` package manager

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/cybergardner/automated-security-incident-response.git
   cd automated-security-incident-response
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On macOS/Linux
   .\venv\Scripts\activate   # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application
1. Start the Flask API server:
   ```bash
   python app/main.py
   ```

2. Test log ingestion with sample data:
   ```bash
   curl -X POST http://127.0.0.1:5000/ingest -H "Content-Type: application/json" -d '{"test": "data"}'
