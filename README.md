# ℹ️Instagram Scraper Cloudflare Worker

A lightweight, zero-dependency Cloudflare Worker that scrapes public Instagram profile data and recent posts using unofficial endpoints. Bypasses many rate limits and works without official API keys.

**Updated for 2026 Instagram changes.**

---
>Live At : https://instainfo.iamaryanbhalsing.workers.dev/info?username=iam._aryanbhalsing
>Note : If it says http error reload site 2-3 time and it will give you response
---

## 🧑‍💻Features

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

## 🔚Endpoints

### `GET /info`

Main endpoint.

**Query Parameters:**
- `username` (required): Instagram username
- `posts` (optional): Number of recent posts to fetch (default: 12, max: 50)
- `highlights` (optional): Set to any value to include story highlights
- `stories` (optional): Set to any value to include current stories

---

## 🍃Limitations & Notes
```
Public accounts only (private accounts will fail).
Instagram frequently changes their web structure — this script includes multiple fallbacks.
Rate limiting may still apply for heavy usage.
Respect Instagram's Terms of Service.
For educational / personal use.
```
---

## ♾️Data Fields (Key ones)
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

## ⚠️Tech Stack

Cloudflare Workers (JavaScript)
Fetch API
Unofficial Instagram web endpoints + GraphQL fallbacks

---

### 📫 Contact & Socials

<p align="center">
  <a href="mailto:aryanbhalsing7090@gmail.com">
    <img src="https://img.shields.io/badge/Email-aryanbhalsing7090%40gmail.com-red?style=for-the-badge&logo=gmail" />
  </a>
  <a href="https://www.linkedin.com/in/iamaryanbhalsing">
    <img src="https://img.shields.io/badge/LinkedIn-iamaryanbhalsing-blue?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="https://github.com/iamaryanbhalsing">
    <img src="https://img.shields.io/badge/GitHub-iamaryanbhalsing-black?style=for-the-badge&logo=github" />
  </a>
  <a href="https://leetcode.com/iamaryanbhalsing">
    <img src="https://img.shields.io/badge/LeetCode-Profile-orange?style=for-the-badge&logo=leetcode" />
  </a>
</p>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=iamaryanbhalsing&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
</p>

---
<img src="https://camo.githubusercontent.com/a5dbb660f658cb0ba61949a83a2eac3bde636395a476ecc7c16124d2a1f9d8a0/68747470733a2f2f73746174732e70706861742e746f702f69636f6e733f6e616d653d6170706c652c617263686c696e75782c646f636b65722c646a616e676f2c666173746170692c6769746c61622c6769742c6769746875622c6a736f6e2c6a6176617363726970742c6c696e75782c6d6f6e676f64622c6e656f76696d2c6e67696e782c706f737467726573716c2c707974686f6e2c727573742c72656163742c72656469732c7461696c77696e646373732c26636f6c756d6e733d3230" />

---

**Thank you for visiting my profile!** ✨  
Let's build something impactful together.
