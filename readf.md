# 🎵 Cubic Music

<div align="center">
  
![Cubic Music Banner](assets/screensho2.jpeg)

### A sleek, modern YouTube Music frontend for Android

[![Latest Version](https://img.shields.io/github/v/release/cybruGhost/Cubic-Music?style=for-the-badge&label=Latest%20Version&color=blue)](https://github.com/cybruGhost/Cubic-Music/releases/latest)
[![Total Downloads](https://img.shields.io/github/downloads/cybruGhost/Cubic-Music/total?style=for-the-badge&label=Total%20Downloads&color=success)](https://github.com/cybruGhost/Cubic-Music/releases)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
[![Crowdin](https://img.shields.io/badge/Crowdin-Translations-2E3340?style=for-the-badge&logo=crowdin)](https://crowdin.com/project/cubic-music)

**Current Version:** `v1.7.9` | **Status:** Beta

</div>

---

## 💖 Support the Project

If you enjoy Cubic Music and want to support development, consider buying me a coffee! Every bit helps keep the project growing 🚀

<div align="center">

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/anonghost40418)

</div>

---

## 📱 Screenshots

<div align="center">
  <img src="assets/screensho2.jpeg" width="280" alt="Cubic Music Screenshot 1"/>
  <img src="assets/scrrenshot.jpeg" width="280" alt="Cubic Music Screenshot 2"/>
</div>

---

## 🎵 About Cubic Music

**Cubic Music** is a powerful, multilingual YouTube Music frontend for Android. It features streaming, full downloads, and stunning visuals—all wrapped in a sleek, modern UI focused on performance and user freedom.

> While it might not be as polished as some mature apps yet, it's a solid, good-looking, and lightweight alternative. The project is maintained and updated as I learn Kotlin skills and add new features!

<div align="center">
  
**⭐ Don't forget to star and follow for updates! ⭐**

</div>

---

## ✨ Key Features

### 🆕 What's New in v1.7.9
| Feature | Description |
|---------|-------------|
| **Spotify Canvas (Beta)** | Short, looping visuals that play instead of static album artwork |
| **Music Rewind** | Your personal listening recap - like Spotify Wrapped! |
| **Spotify Playlists** | Import your favorite Spotify playlists directly |
| **Explicit Tags** | Clear labeling for explicit content |

### 🎧 Core Features
- **Smart Caching** - Custom cache size for offline listening
- **Batch Downloads** - Download entire playlists at once
- **Offline Mode** - Works without internet connection
- **Background Playback** - Listen while using other apps
- **Listening Statistics** - Track your music habits
- **Audio Visualizer** - Multiple visualizer styles to choose from

### 📝 Lyrics & Playlists
- **Lyrics Support** - Fetch, edit, translate, synced/unsynced lyrics
- **Playlist Management** - Import/Export playlists (RiMusic compatible)
- **Import Backups** - Seamlessly import from RiMusic

### 🎨 Customization
- **Dynamic Themes** - Adapts to your style
- **Sleep Timer** - Fully customizable auto-stop
- **Audio Controls** - Playback speed, pitch, volume, normalization
- **Skip Silence** - Toggle to remove silent gaps

### 📱 Platform Support
- **Android Auto** - Drive safely with music controls
- **Android TV** - Big screen experience
- **Widgets** - *(Experimental)* Quick access from home screen

### ⚙️ Utilities
- **Update Checker** - Toggle in settings to check for new versions
- **Export Options** - Export settings, downloads, and cached media
- **Multi-language** - Expanding localization support

---

## 📊 Download Statistics

<div align="center">

### Live Download Counters

| Metric | Downloads |
|--------|-----------|
| **All-Time Downloads** | [![Total Downloads](https://img.shields.io/github/downloads/cybruGhost/Cubic-Music/total?label=Total&color=blue)](https://github.com/cybruGhost/Cubic-Music/releases) |
| **Current Release (v1.7.9)** | [![Latest Release Downloads](https://img.shields.io/github/downloads/cybruGhost/Cubic-Music/latest/total?label=v1.7.9&color=green)](https://github.com/cybruGhost/Cubic-Music/releases/latest) |
| **All Releases** | [![All Releases](https://img.shields.io/github/downloads/cybruGhost/Cubic-Music/total?label=All%20Versions&color=orange)](https://github.com/cybruGhost/Cubic-Music/releases) |

</div>

---

## 🔮 Roadmap

- [ ] Improved playlist mood detection
- [ ] Memory optimization for large caches
- [ ] UI refinements (RiMusic-inspired improvements)
- [ ] Enhanced localization support
- [ ] Performance optimizations

---

## 📥 Playlist Import Formats

Cubic Music supports multiple playlist formats for maximum compatibility.

### 📋 Supported Formats

<details>
<summary><b>🧩 Compatible App Format (Native)</b></summary>

```csv
PlaylistBrowseId,PlaylistName,MediaId,Title,Artists,Duration,ThumbnailUrl
,Swipefy,1pEe7-tWv2M,Good Grief,Jenna Raine,160,https://inv.perditum.com/vi/1pEe7-tWv2M/hqdefault.jpg
Required: PlaylistName, MediaId, Title, Artists, Duration

</details><details> <summary><b>🧱 Extended App Format (With Album Info)</b></summary>
csv
PlaylistBrowseId,PlaylistName,MediaId,Title,Artists,Duration,ThumbnailUrl,AlbumId,AlbumTitle,ArtistIds
,MyPlaylist,abc123,Song Title,Artist Name,180,https://example.com/thumb.jpg,album123,Album Name,artist123
</details><details> <summary><b>🎧 Spotify Export Format</b></summary>
csv
Track Name,Artist Name(s),Track Duration (ms),Album Name,Album Image URL,Explicit
Blinding Lights,The Weeknd,200040,After Hours,https://i.scdn.co/image/ab67616d0000b273,false
</details><details> <summary><b>💽 Exportify Format</b></summary>
csv
Track URI,Track Name,Artist Name(s),Album Name,Album Image URL,Track Duration (ms),Explicit,Playlist Name
spotify:track:123,Blinding Lights,The Weeknd,After Hours,https://i.scdn.co/image/ab67616d0000b273,200040,false,My Spotify Playlist
</details><details> <summary><b>🪶 Custom Format (Minimal)</b></summary>
csv
PlaylistBrowseId,PlaylistName,MediaId,Title,Artists,Duration
,MyPlaylist,abc123,Song Title,Artist Name,180
</details>
⚙️ Import Processing
✅ Compatible Formats - Imported directly (App, Extended, Custom)

🔄 Conversion Formats - Converted to YouTube tracks (Spotify, Exportify)

📊 API Status
<div align="center">
Service	Status
API	https://img.shields.io/badge/dynamic/json?label=API&query=$.0.type&url=https://yt.omada.cafe/api/v1/search?q=test&color=brightgreen
Search	https://img.shields.io/badge/dynamic/json?label=Search&query=$.0.type&prefix=OK&url=https://yt.omada.cafe/api/v1/search?q=test
Results	https://img.shields.io/badge/dynamic/json?label=Results&query=$.length&url=https://yt.omada.cafe/api/v1/search?q=test
</div>
⚖️ Legal & Disclaimer
Legal Notice
Cubic Music respects music copyrights and does not enable illegal downloads. All content is streamed via licensed APIs or legitimate external sources only.

Disclaimer
This project is not affiliated with, endorsed by, or sponsored by YouTube, Google LLC, or their affiliates. All trademarks and intellectual property belong to their respective owners.

👨‍💻 About the Developer
<div align="center">
Made with ❤️ by a learner — cybruGhost

Cubic Music is a passion project, built and maintained as I grow my Kotlin skills. Every star, follow, and contribution means the world! 🌟

https://img.shields.io/github/followers/cybruGhost?style=social
https://img.shields.io/github/stars/cybruGhost/Cubic-Music?style=social

⭐ Star this repo to show support! ⭐

Last updated: February 2026

</div> ```
