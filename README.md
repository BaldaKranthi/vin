# Video Steganography with Encryption

This Django project allows you to encrypt messages and embed them into a video file using steganography. You can also decrypt and extract the embedded messages from the video files.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Explanation of Core Functions](#explanation-of-core-functions)
- [Templates](#templates)
- [License](#license)

## Prerequisites

- Python 3.x
- Django 3.x or higher
- OpenCV (cv2)
- NumPy

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/videosteganography.git
    cd videosteganography
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Apply migrations:
    ```sh
    python manage.py migrate
    ```

5. Run the Django development server:
    ```sh
    python manage.py runserver
    ```

6. Open your web browser and navigate to `http://127.0.0.1:8000`.

## Usage

### Encrypt a Message in a Video

1. Go to the encryption page (`/encrypt`).
2. Enter the message you want to encrypt.
3. Provide an encryption key.
4. Upload the video file where you want to embed the message.
5. Click on "Encrypt".
6. The page will display the encoded video which you can download.

### Decrypt a Message from a Video

1. Go to the decryption page (`/decrypt`).
2. Provide the decryption key.
3. Upload the video file from which you want to extract the message.
4. Click on "Decrypt".
5. The page will display the decrypted message.

## Project Structure

