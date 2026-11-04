# Third-Party Notices — Nova Video Downloader

Nova Video Downloader is proprietary freeware (see `LICENSE.txt`). It includes or uses the following third-party components, each under its own license. Full license texts are in the `licenses/` folder.

## FFmpeg 7.1 — GPLv3
- Bundled through the `imageio-ffmpeg` 0.6.0 package (BSD-2-Clause) as `ffmpeg-win-x86_64-v7.1.exe`.
- This build is configured with `--enable-gpl --enable-version3 --enable-libx264` and is therefore licensed under **GNU GPL version 3**. See `licenses/GPL-3.0.txt`.
- Nova Video Downloader runs FFmpeg only as a **separate program** (command-line process); it is not linked into the application.
- Website: https://ffmpeg.org — Source code: https://ffmpeg.org/releases/ffmpeg-7.1.tar.xz
- x264 source: https://code.videolan.org/videolan/x264
- **Written offer:** for at least three years from the date of each release, the developer will provide the complete corresponding source code of the bundled FFmpeg binary to anyone who asks (contact X: @qqussaai). The FFmpeg source archive is also attached to the GitHub release.
- FFmpeg is a trademark of Fabrice Bellard. This software is not endorsed by the FFmpeg project.

## Qt 6 / PySide6 — LGPLv3
- Used as the GUI toolkit (PySide6 6.x). License: `licenses/LGPL-3.0.txt`.
- Source: https://download.qt.io/official_releases/QtForPython/ and https://code.qt.io
- You may replace the Qt/PySide6 libraries with your own compatible versions as permitted by the LGPL.

## yt-dlp — Unlicense
- Used for downloading. License: `licenses/yt-dlp-Unlicense.txt`. https://github.com/yt-dlp/yt-dlp
- Related packages (yt-dlp-ejs, Brotli, PyCryptodomex, websockets) are listed under "Other components" below.

## whisper.cpp and the Whisper model — MIT (optional, downloaded on first use)
- Used only for "AI auto-subtitles". Nothing is bundled in the installer: when the user turns the option on, the app asks first, then downloads the pinned files and verifies their SHA-256 before use.
- whisper.cpp release `b5454` (`whisper-bin-x64.zip`) from https://github.com/ggml-org/whisper.cpp — License: `licenses/whisper.cpp-MIT.txt`. Runs as a **separate program** (command-line process).
- Model `ggml-large-v3-turbo-q5_0.bin` from https://huggingface.co/ggerganov/whisper.cpp, converted from OpenAI Whisper — License: `licenses/openai-whisper-MIT.txt`.

## HT-Demucs vocal separation model — MIT (optional, downloaded on first use)
- Used only for "Separate vocals from music". Nothing is bundled in the installer: when the user turns the option on, the app asks first, then downloads the pinned file and verifies its SHA-256 before use.
- Model `htdemucs_ft_vocals_fp16weights.onnx` from https://huggingface.co/StemSplitio/htdemucs-ft-vocals-onnx, an ONNX conversion of Demucs (HT-Demucs) by Meta, https://github.com/facebookresearch/demucs — License: `licenses/demucs-MIT.txt`.

## ONNX Runtime — MIT
- Bundled (CPU build) to run the separation model. License: `licenses/onnxruntime-MIT.txt`, third-party notices: `licenses/onnxruntime-ThirdPartyNotices.txt`. https://github.com/microsoft/onnxruntime

## NumPy — BSD-3-Clause
- Bundled for audio processing. License: `licenses/numpy-BSD-3-Clause.txt`. https://numpy.org

## Tajawal font — SIL OFL 1.1
- Bundled in the app (Regular, Medium, Bold) and used for the interface. Copyright 2018 Boutros International. License: `licenses/Tajawal-OFL-1.1.txt`. https://github.com/googlefonts/tajawal

## Other components
Full license texts for the Python packages below are in `licenses/python-packages-licenses.txt`.

| Component | License |
|---|---|
| Python runtime (including its bundled OpenSSL, libffi, SQLite, expat) | PSF License; OpenSSL Apache-2.0; libffi MIT; SQLite public domain; expat MIT |
| certifi | MPL-2.0 (`licenses/MPL-2.0.txt`), https://github.com/certifi/python-certifi |
| requests | Apache-2.0 |
| urllib3 | MIT |
| charset-normalizer | MIT |
| idna | BSD-3-Clause |
| websockets | BSD-3-Clause |
| Brotli | MIT |
| PyCryptodomex | BSD-2-Clause and Public Domain |
| yt-dlp-ejs (JavaScript helpers for yt-dlp) | Unlicense AND MIT AND ISC |
| imageio-ffmpeg | BSD-2-Clause |
| NumPy, including its bundled OpenBLAS (`licenses/numpy-BSD-3-Clause.txt`) | BSD-3-Clause and others, listed in that file |
| SymPy, mpmath, flatbuffers (installed with ONNX Runtime) | BSD-3-Clause, BSD-3-Clause, Apache-2.0 |
| packaging | Apache-2.0 OR BSD-2-Clause |
| setuptools | MIT |
| PyInstaller (bootloader) | GPL-2.0 with exception allowing use for any program |
