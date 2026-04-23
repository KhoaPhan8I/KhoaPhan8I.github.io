# TikTok App Review Package

## Products and scopes explanation

Vua Thợ Media Hub uses TikTok Login Kit and Display API only after the user explicitly authorizes the app. The app requests user.info.basic to confirm the connected TikTok account and video.list to retrieve metadata and cover images of the authorized user's public videos. These TikTok video covers are imported into a local media review library where the user can review, score, deduplicate, and decide whether to use them for internal content planning. The app does not post to TikTok, does not scrape TikTok public pages, does not download private data, and does not access accounts that have not authorized the app.

## Demo video script

1. Open `https://khoaphan8i.github.io/`.
2. Open the local app at `http://127.0.0.1:8000/connections`.
3. Show TikTok client configuration and click `Connect TikTok`.
4. Login and authorize TikTok scopes `user.info.basic` and `video.list`.
5. Return through `https://khoaphan8i.github.io/tiktok/callback`.
6. Click `Open local app` to finish token exchange.
7. Show TikTok status as connected in `Connections`.
8. Create a `tiktok_video_covers` source in `Sources`.
9. Run `Discover` in `Jobs`.
10. Open `Library` or `Review` and show TikTok video cover metadata imported for review.

Export as MP4/MOV under 50MB before uploading to TikTok Developer Portal.
