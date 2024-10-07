# Gemini Pro Vision - Text and Image Query Application

This is a Streamlit application that uses Google Generative AI to process both text and image inputs. The application loads environment variables using `python-dotenv` for secure management of sensitive information like API keys. It supports processing natural language questions, image analysis, or both using the appropriate models from Google's Generative AI (Gemini Pro and Gemini Pro Vision).

## Features

- **Text and Image Processing**: Handle questions and images through Generative AI models.
- **Secure API Key Management**: Environment variables are loaded using `dotenv`.
- **Image Upload**: Allows users to upload images for analysis by the Gemini Pro Vision model.
- **Multi-Input Support**: You can input text, images, or both for different use cases.

## Prerequisites

1. Python 3.x
2. Streamlit
3. [Google Generative AI](https://developers.generativeai.google)
4. [Python-Dotenv](https://pypi.org/project/python-dotenv/)
5. PIL (Pillow for image processing)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/gemini-pro-vision-app.git
    cd gemini-pro-vision-app
    ```

2. Install the required dependencies:
    ```bash
    pip install streamlit google-generativeai python-dotenv pillow
    ```

3. Set up your environment:
    - Create a `.env` file in the project root directory and add your **Google Generative AI** API key as follows:
      ```
      GOOGLE_API_KEY=your-google-api-key
      ```

4. Ensure the `student.db` SQLite database is set up, or generate a dummy one using the provided function.

## Running the Application

To run the Streamlit application, execute the following command:

```bash
streamlit run app.py
