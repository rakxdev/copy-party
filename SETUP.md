# Setup Instructions for `copyparty` Telegram Uploader

This guide will help you set up and run the `copyparty` server.

### 1. Install System Dependencies

You need to install `ffmpeg`, which is crucial for handling large media files. On a Debian-based system (like Ubuntu), you can do this with:

```bash
sudo apt-get update
sudo apt-get install -y ffmpeg
```

### 2. Install Python Dependencies

The required Python library is listed in `requirements.txt`. Install it using pip from the root of this project:

```bash
pip3 install -r requirements.txt
```

### 3. Create the Uploads Directory

The server configuration expects an `uploads` directory to exist. Create it now:
```bash
mkdir uploads
```

### 4. Run the Server

Once the dependencies are installed, you can start the server. Make sure you are in the root of this project, then run:

```bash
./copyparty-sfx.py -c copyparty.conf
```

The server will start, and you can access it at `http://YOUR_VPS_IP:3923`. Uploaded files will be processed by `telegram_uploader.py`.
