# Securing Data Using Cryptography and Steganography Techniques

This Django project allows you to secure data using a combination of cryptography and steganography techniques. It supports embedding and extracting encrypted messages in various media types, including images, videos, and audio, as well as encoding messages in Morse code and emojis.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
  - [Encrypt and Embed Message in an Image](#encrypt-and-embed-message-in-an-image)
  - [Decrypt and Extract Message from an Image](#decrypt-and-extract-message-from-an-image)
  - [Encrypt and Embed Message in a Video](#encrypt-and-embed-message-in-a-video)
  - [Decrypt and Extract Message from a Video](#decrypt-and-extract-message-from-a-video)
  - [Encrypt and Embed Message in Audio](#encrypt-and-embed-message-in-audio)
  - [Decrypt and Extract Message from Audio](#decrypt-and-extract-message-from-audio)
  - [Convert Message to Morse Code](#convert-message-to-morse-code)
  - [Convert Morse Code to Message](#convert-morse-code-to-message)
  - [Convert Message to Emoji](#convert-message-to-emoji)
  - [Convert Emoji to Message](#convert-emoji-to-message)
- [Project Structure](#project-structure)
- [Explanation of Core Functions](#explanation-of-core-functions)
- [Templates](#templates)
- [License](#license)

## Prerequisites

- Python 3.x
- Django 3.x or higher
- OpenCV (cv2)
- NumPy
- Pillow (PIL)
- Any additional libraries required for audio processing

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/securingdata.git
    cd securingdata
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

### Encrypt and Embed Message in an Image

1. Go to the encryption page (`/encrypt_image`).
2. Enter the message you want to encrypt.
3. Provide an encryption key.
4. Upload the image file where you want to embed the message.
5. Click on "Encrypt".
6. The page will display the encoded image which you can download.

### Decrypt and Extract Message from an Image

1. Go to the decryption page (`/decrypt_image`).
2. Provide the decryption key.
3. Upload the image file from which you want to extract the message.
4. Click on "Decrypt".
5. The page will display the decrypted message.

### Encrypt and Embed Message in a Video

1. Go to the encryption page (`/encrypt_video`).
2. Enter the message you want to encrypt.
3. Provide an encryption key.
4. Upload the video file where you want to embed the message.
5. Click on "Encrypt".
6. The page will display the encoded video which you can download.

### Decrypt and Extract Message from a Video

1. Go to the decryption page (`/decrypt_video`).
2. Provide the decryption key.
3. Upload the video file from which you want to extract the message.
4. Click on "Decrypt".
5. The page will display the decrypted message.

### Encrypt and Embed Message in Audio

1. Go to the encryption page (`/encrypt_audio`).
2. Enter the message you want to encrypt.
3. Provide an encryption key.
4. Upload the audio file where you want to embed the message.
5. Click on "Encrypt".
6. The page will display the encoded audio file which you can download.

### Decrypt and Extract Message from Audio

1. Go to the decryption page (`/decrypt_audio`).
2. Provide the decryption key.
3. Upload the audio file from which you want to extract the message.
4. Click on "Decrypt".
5. The page will display the decrypted message.

### Convert Message to Morse Code

1. Go to the Morse code conversion page (`/morse_code`).
2. Enter the message you want to convert.
3. Provide an encryption key.
4. Click on "Convert".
5. The page will display the Morse code representation of the message.

### Convert Morse Code to Message

1. Go to the Morse code decryption page (`/morse_code_decrypt`).
2. Enter the Morse code you want to convert back to the original message.
3. Provide the decryption key.
4. Click on "Decrypt".
5. The page will display the original message.

### Convert Message to Emoji

1. Go to the emoji conversion page (`/emoji_convert`).
2. Enter the message you want to convert.
3. Provide an encryption key.
4. Click on "Convert".
5. The page will display the emoji representation of the message.

### Convert Emoji to Message

1. Go to the emoji decryption page (`/emoji_decrypt`).
2. Enter the emoji string you want to convert back to the original message.
3. Provide the decryption key.
4. Click on "Decrypt".
5. The page will display the original message.

## Project Structure

