---
name: get-started
description: How to make a first AI video with Revana in ChatGPT - check the balance, get a free quote, confirm the price with the user, make the video and share the download link.
---

# Get started with Revana

Revana makes AI videos (Seedance 2.5) on the user's Revana account, using credits they already have.

1. Ask what the video should show, and the resolution (480p, 720p or 1080p), length in seconds and aspect ratio.
2. Call `get_balance` to see what the account can spend, then `get_quote` for the exact price. Both are free.
3. Tell the user the price and wait for a clear yes before calling `generate_video`.
4. Videos take one to several minutes. Call `get_video` (with `wait_seconds`) until it succeeds, then share the link from `get_video_link`.
5. Failed videos are not charged. To restage an existing clip with other people, products or places, use `quote_nemesis` and then `make_nemesis`, also quoted first.
