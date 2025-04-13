# Eleventh Hour

![Eleventh Hour Banner](static/images/banner1.jpg)

Welcome to **Eleventh Hour**, a Flask web app designed to make code documentation a breeze. Ever need to analyze your code and whip up a polished project report at the last minute? This tool's got your back. Upload your code, let AI break it down with summaries and flowcharts, add some project details, and boom—you've got a professional Word doc ready to go. It's built for developers who want to showcase their work without getting bogged down in report-writing.

## Features

- **Code Upload**: Handles a bunch of file types like `.py`, `.js`, `.jsx`, `.ts`, `.java`, and more.
- **AI-Powered Analysis**: Uses Google Gemini AI to generate summaries, descriptions, and flowcharts for your code.
- **Project Details**: Collects info like project title, teammates, and goals through a simple form.
- **Document Generation**: Creates a Word doc with a title page, certificate, abstract, methodology, results, and more.
- **Flowcharts**: Auto-generates visual flowcharts for each file using Mermaid CLI.
- **PDF Export**: Download a PDF version of the analysis (basic for now, but handy).
- **Sleek UI**: Light/dark mode toggle for those late-night coding sessions.

## Prerequisites

- Python 3.8 or higher
- Node.js (for Mermaid CLI)
- A Google Gemini API key (grab one from [Google AI Studio](https://aistudio.google.com/))
- Dependencies listed in `requirements.txt`

## Installation

1. **Clone the Repo**:

   ```bash
   git clone https://github.com/your-username/eleventh-hour.git
   cd eleventh-hour

   ```

2. **Set Up a Virtual Environment**:

   ```bash
   python -m venv venv
   venv\Scripts\activate # Windows
   source venv/bin/activate  # Mac or Linux

   ```

3. **Install Python Dependencies**:

   ```bash
   pip install -r requirements.txt

   ```

4. **Install Mermaid CLI**:

   ```bash
   npm install -g @mermaid-js/mermaid-cli

   ```

5. **Set Up Environment Variables**:
   Create a .env file in the project root:
   ```bash
   GEMINI_API_KEY=your-gemini-api-key
   ```

## Usage

1. **Start the App**:

   - Run the command: python app.py
   - It'll launch at http://localhost:5000. Simple as that.

2. **How It Works**:

   - **Upload Code**: Drop in your files—things like .py, .js, or others (up to 20 files, 10MB total).
   - **Check Analysis**: See AI-powered summaries, descriptions, and flowcharts for each file.
   - **Fill in Details**: Add project info like title, your name, teammates, and the project's goal.
   - **Generate Doc**: Download a Word doc with a title page, analysis, flowcharts, and all the good stuff.

3. **Example**:
   - Upload a file like App.js for a React app.
   - Enter details: Project Title: "Packing List Manager", Author: "Vamsi Krishna", Goal: "Make packing for trips easier".
   - Get final_document.docx with everything organized and ready to roll.
