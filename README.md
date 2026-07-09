# ℹ️Instagram Scraper Cloudflare Worker

A lightweight, zero-dependency Cloudflare Worker that scrapes public Instagram profile data and recent posts using unofficial endpoints. Bypasses many rate limits and works without official API keys.

**Updated for 2026 Instagram changes.**

---
>Live At : https://instainfo.iamaryanbhalsing.workers.dev/info?username=iam._aryanbhalsing
---

## Features

- **Profile Information**: Full user profile with bio, stats, links, business info, etc.
- **Recent Posts**: Fetch up to 50 recent posts (photos, videos, carousels, reels).
- **Media Details**: Rich metadata including:
  - Images, videos, carousels
  - Music (original audio, tracks)
  - Location, sponsors, tagged users
  - Captions, hashtags, comments preview
- **Highlights & Stories** (optional): Story highlights and current stories.
- **CORS Enabled**: Ready for frontend use.
- **Robust**: Multiple fallback methods for data extraction.

---

## Endpoints

### `GET /info`

Main endpoint.

**Query Parameters:**
- `username` (required): Instagram username
- `posts` (optional): Number of recent posts to fetch (default: 12, max: 50)
- `highlights` (optional): Set to any value to include story highlights
- `stories` (optional): Set to any value to include current stories

---

## Limitations & Notes

Public accounts only (private accounts will fail).
Instagram frequently changes their web structure — this script includes multiple fallbacks.
Rate limiting may still apply for heavy usage.
Respect Instagram's Terms of Service.
For educational / personal use.

---

## Data Fields (Key ones)
```Profile

Bio, external links, business contact info
Follower/following counts
Verification status
Pinned channels, AI agent info, etc.

Posts

Media URLs (images/videos)
Caption, hashtags, location
Engagement metrics (likes, comments, views)
Music attribution
Tagged users, co-authors
```

## Tech Stack

Cloudflare Workers (JavaScript)
Fetch API
Unofficial Instagram web endpoints + GraphQL fallbacks

License
MIT - Free to use, modify, and deploy.

