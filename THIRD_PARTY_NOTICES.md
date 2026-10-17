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
- Related: `yt-dlp-ejs`, `brotli` (MIT), `pycryptodomex` (BSD/Public Domain), `websockets` (BSD-3-Clause).

## Other components
| Component | License |
|---|---|
| Python | PSF License |
| certifi | MPL-2.0 (`licenses/MPL-2.0.txt`), https://github.com/certifi/python-certifi |
| requests | Apache-2.0 |
| urllib3 | MIT |
| imageio-ffmpeg | BSD-2-Clause |
| PyInstaller (bootloader) | GPL-2.0 with exception allowing use for any program |
