# Gemini-App-To-Retrieve-SQL-Data
Gen AI Project


This project allows users to ask questions in plain English about a SQLite database containing student records. The application uses Google Generative AI to convert these questions into SQL queries and retrieve the relevant data.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Requirements](#requirements)
- [License](#license)

## Features
- Upload and query a SQLite database.
- Convert plain English questions into SQL queries using Google Generative AI.
- Retrieve and display the results from the SQLite database.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Gemini_App_To_Retrieve_SQL_Data.git
    cd Gemini_App_To_Retrieve_SQL_Data
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your API key:
    - Create a `.env` file in the project directory.
    - Add your Google API key to the `.env` file:
      ```
      GOOGLE_API_KEY=your_google_api_key
      ```

5. Set up the SQLite database:
    - Run the `sql.py` script to create and populate the `student.db` database:
      ```bash
      python sql.py
      ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. In the Streamlit interface:
    - Enter your question in plain English in the text input box.
    - Click on "Ask the question" to get a response based on the content of the SQLite database.

## Requirements

- Python 3.x
- streamlit
- google-generativeai
- python-dotenv

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
