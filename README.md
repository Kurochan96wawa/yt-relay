# yt-relay

A one-file relay page for watching YouTube videos from local HTML notes.

A page opened as a local file (`file://`) sends no `Referer`, so YouTube's embedded player refuses it (Error 153).
`index.html` here embeds the YouTube player; a local page embeds this page instead:

    https://kurochan96wawa.github.io/yt-relay/?v=VIDEO_ID

It only accepts an 11-character YouTube video ID and renders the standard `youtube-nocookie.com` embed. No tracking, no data.
