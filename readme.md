# [Youtube Chapters Chrome Extension](https://youtubechapters.app)

[Youtubechapters.app](https://youtubechapters.app) is used by thousands of people every month, this repo contains a Chrome extension that helps you quickly generate a summary. It'll take you to by youtube chapters page. The summary provides a overview of the video's content, allowing you to understand the main points without watching the entire video. You can copy the summary, copy only the chapters (if you leave it as a comment you'll get links), and you can share the summary link as well.

## Also! If you want to use your own openai key call this for free.

```sh 
curl --no-buffer -X 'POST' \
  'https://youtube-markdown.fly.dev/youtube_markdown'\
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -H 'Authorization: Bearer (openai-api-key)' \
  -d '{
  "use_cache": false,
  "url": "https://www.youtube.com/watch?v=QmOF0crdyRU&t=2s",
  "use_sse": false 
}'
```

## Features

- Adds a button to the Chrome toolbar, accessible when viewing a YouTube video.
- One-click to open a new tab with a summary of the current YouTube video.
- Automatically generates the summary using the magic URL: `https://magic.jxnl.co/youtube?v=<videoId>`.

## Installation

### Manual Installation 

1. Clone or download this repository to your local machine.
2. Open Google Chrome and navigate to `chrome://extensions/`.
3. Enable "Developer mode" by toggling the switch in the top right corner.
4. Click "Load unpacked" and select the folder containing the YouTube Summarizer extension.
5. The YouTube Summarizer extension should now be installed and visible in your Chrome toolbar.

## Usage

1. Visit a YouTube video page, such as `https://www.youtube.com/watch?v=abcdefghijk`.
2. Click the YouTube Summarizer button in your Chrome toolbar.
3. A new tab will open with the magic URL, e.g., `https://magic.jxnl.co/youtube?v=abcdefghijk`.
4. View the generated summary of the YouTube video.

## Contributing

Feel free to contribute to this project by submitting issues, feature requests, or pull requests.


