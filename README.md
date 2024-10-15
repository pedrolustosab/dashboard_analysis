# Dashboard Analyzer AI

## Description

Dashboard Analyzer AI is a Python-based tool that automatically analyzes dashboard images, generates comprehensive summaries, and saves the analysis in a markdown file. This tool uses advanced AI capabilities to interpret visual elements of dashboards, providing insights on layout, functionality, and potential improvements.

## Features

- Scans the current working directory for dashboard images (jpg or png)
- Analyzes each dashboard image using AI
- Generates detailed summaries including:
  - Buttons and clickable elements
  - Cards and containers
  - Charts and visual representations
  - Tables and matrices
  - Overall layout and structure
  - Inferred purpose of the dashboard
  - Key insights from the data
  - Suggestions for UI/UX improvements
- Saves all analyses in a single markdown file

## Requirements

- Python 3.x
- Required Python packages:
  - os
  - re
  - base64
  - io
  - PIL (Python Imaging Library)
  - python-dotenv
  - langchain
  - openai

## Setup

1. Clone this repository to your local machine.
2. Install the required packages:
   ```
   pip install python-dotenv pillow langchain openai
   ```
3. Set up your OpenAI API key in a `.env` file:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

1. Place your dashboard images (jpg or png) in the same directory as the script.
2. Run the Jupyter notebook or Python script.
3. The AI will automatically:
   - Detect dashboard images in the directory
   - Analyze each image
   - Generate summaries
   - Save all analyses in a file named `dashboard_analysis.md`

## Functions

- `list_of_files(extension)`: Lists all files with a specific extension in the current directory.
- `generate_image_summary(image_path)`: Analyzes a dashboard image and generates a detailed summary.
- `save_to_markdown(summary, filename)`: Saves the generated summaries to a markdown file.

## Note

This tool uses OpenAI's GPT-4 model for image analysis. Ensure you have the necessary API access and credits available.

