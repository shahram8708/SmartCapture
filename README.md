# Smart Capture

**Smart Capture** is a web application for capturing video, uploading it for processing, and receiving a textual summary of the video's content. The application utilizes Flask for the backend and integrates with Google's Generative AI to analyze video content.

## Features

- **Video Recording**: Capture video using your webcam.
- **Video Upload**: Upload recorded video for processing.
- **Text Summary**: Receive a textual summary of the video's content.
- **Audio Playback**: Play and stop audio readouts of the response.
- **Clipboard Copy**: Copy the response text to the clipboard.
- **Responsive Design**: Professional and user-friendly design.

## Requirements

- Python 3.7 or higher
- Flask
- Google Generative AI
- Markdown

## Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/shahram8708/SmartCapture
   cd SmartCapture
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**

   - **Windows:**

     ```bash
     venv\Scripts\activate
     ```

   - **macOS/Linux:**

     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

5. **Set Up Environment Variables**

   Create a `.env` file in the root directory of your project and add your Google Generative AI API key:

   ```plaintext
   API_KEY=your_google_generative_ai_api_key
   ```

6. **Run the Application**

   ```bash
   python app.py
   ```

   The application will start running on `http://127.0.0.1:5000/`.

## Usage

1. Open the application in your web browser.
2. Click **Start** to begin recording a video.
3. Click **Stop** when you’re done recording.
4. The recorded video will be uploaded for processing.
5. After processing, a textual summary will be displayed.
6. Use the **Play Audio** and **Stop Audio** buttons to hear the summary read aloud.
7. Click **Copy Response** to copy the summary text to your clipboard.

## Directory Structure

```
/project-root
    /uploads
    app.py
    requirements.txt
    .env
    templates/
        index.html
```

## Troubleshooting

- **Error uploading video**: Ensure the video file is correctly recorded and try again.
- **No response**: Check if the API key is correctly set up and valid.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

- [Flask](https://flask.palletsprojects.com/)
- [Google Generative AI](https://developers.google.com/generative-ai)
- [Markdown](https://python-markdown.github.io/)

For any issues or contributions, please open an issue or submit a pull request on the project's GitHub repository.
