# Drive Index Video Playlist Generator

This script crawls a Google Drive index and generates `.m3u` playlists containing direct links to video files found in each folder.

## Features

* Recursively scans folders
* Detects common video formats (`.mp4`, `.mkv`, `.avi`, `.mov`, `.webm`)
* Generates one `.m3u` playlist per top-level folder

## Requirements

* Python 3.8+
* `requests` library

Install dependencies:

```bash
pip install requests
```

## Usage

1. Update `BASE_INDEX` if needed to point to your Drive index URL.
2. Run the script:

```bash
python crawler.py
```

3. Generated `.m3u` files will appear in the current directory.

Each playlist can be opened in media players like VLC, MPV or Kodi.

## Configuration

* `VIDEO_EXT`: File extensions treated as videos
* `max_depth` (in `crawl`): Limits recursion depth
* `ROOT_PATH`: Starting directory (default is root)

## Notes

* This script assumes a public Drive index with JSON responses.
* Performance depends on index size and server rate limits.

## 👨‍💻 Author

**NIKHIL** ([8nikhil](https://github.com/8nikhil))
- Email: [8nikhil282005@gmail.com](mailto:8nikhil282005@gmail.com)
- GitHub: [https://github.com/8nikhil](https://github.com/8nikhil)
