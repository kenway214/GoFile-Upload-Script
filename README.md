# GoFile Uploader Script
A simple script to upload files to https://gofile.io

## Usage:
```bash
./upload.sh <path/to/file>
```
You'll see the link after the upload completes.

## One-shot install (bash)
```bash
wget -q https://raw.githubusercontent.com/kenway214/GoFile-Upload-Script/master/upload.sh -O ~/gofile && chmod +x ~/gofile
echo 'alias gofile="~/gofile"' >> ~/.bashrc && source ~/.bashrc
```
Then run:
```bash
gofile <path/to/file>
```

## Features:
- Upload files to https://gofile.io using their API


## Requirements:
- `curl` and `jq` must be installed.

## Based on
- Original script: https://github.com/Sushrut1101/GoFile-Upload

## Changes in this version
- Added basic error handling and clearer output.
- Uses the server list API to pick the first available server.
- Temporary `-k` on `curl` for environments that need it.

## Credits:
- https://gofile.io - For the amazing website to upload unlimited files, for free.
