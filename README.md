# Audio Transcriber Backend

This Spring Boot backend service converts MP3 audio files to text using OpenAI's models. It is intended for integration with a frontend application.

## Features

- Upload MP3 files
- Convert audio to text
- Retrieve transcriptions

## Prerequisites

- JDK 11 or later
- Maven
- OpenAI API key

## Setup and Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/audio-transcriber-backend.git
   cd audio-transcriber-backend
   ```

2. **Configure Application Properties**

   Add your OpenAI API key to `src/main/resources/application.properties`:

   ```properties
   openai.api.key=YOUR_OPENAI_API_KEY
   ```

3. **Build and Run**

   Build the project:

   ```bash
   mvn clean package
   ```

   Start the application:

   ```bash
   mvn spring-boot:run
   ```

   The service will run on port 8080 by default.

## Integration

To use this service, connect your frontend application to the `/api/transcribe` endpoint for processing MP3 files. For the frontend application, visit the [frontend repository](https://github.com/Jonathan-Tong1/audio-transcriber).
