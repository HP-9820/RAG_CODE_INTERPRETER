# Code Interpreter Streamlit App

A simple **Streamlit** application that generates Python code based on user input and executes the code either locally or in a Docker container.

## Features

- **Code Generation**: Users can input a prompt, and the app will generate the Python code to fulfill the request.
- **Execution Environments**:
  - **Local Execution**: Runs the generated code on the user's local machine.
  - **Docker Execution**: Runs the generated code inside a Docker container.
- **Google Cloud Integration**: Uses Google Cloud's `ChatGoogleGenerativeAI` model for code generation.
- **File Upload**: Allows execution of generated code with the option of uploading necessary files.
- **Visual Output**: If the generated code creates charts or images, it will display them in the app.

## Prerequisites

Before running the app, ensure that the following prerequisites are met:

- **Google Cloud API Credentials**:
  - Ensure that you have a Google Cloud account and that you've enabled the necessary APIs.
  - Download the `client_secret_XXXXXX.json` file from your Google Cloud project.
  - Set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to point to your JSON credentials file.

  Example:
  ```bash
  export GOOGLE_APPLICATION_CREDENTIALS="C:\\Users\\your_username\\Downloads\\client_secret_XXXXXX.json"

