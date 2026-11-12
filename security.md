# Mangadotnet Manga Downloader

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0F0C29,100:E94040&height=220&section=header&text=Mangadotnet%20Manga%20Downloader&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Build%20Your%20Ultimate%20Offline%20Manga%20Library&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-3.4.0-E94040?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-98.6K-0F0C29?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FFD700?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-00C9FF?style=for-the-badge&logo=python&logoColor=white)

</div>

---

## 📖 The End Of The Loading Screen

Reading manga online is a frustrating experience. You are constantly interrupted by intrusive ads, the pages load slowly, and if the website goes down, your favorite series disappears overnight. For true manga enthusiasts, the only real solution is to own your library.

**Mangadotnet Manga Downloader** is a fast, lightweight, and open-source command-line tool designed to archive manga from popular sources. It is not just a simple image scraper; it is a complete library management system.

This repository provides a highly optimized Python script that handles the entire workflow. You give it a URL, and it automatically fetches the chapter metadata, downloads the high-resolution images, sorts them into folders, and even compiles them into `.cbz` (Comic Book Archive) files. These `.cbz` files are universally supported by readers like Tachiyomi, Perfect Viewer, and even Apple Books. It is the ultimate tool for data hoarders and dedicated fans.

<img width="512" height="250" alt="mangaPreview" src="https://github.com/user-attachments/assets/aace2ef5-8f2c-472b-a9f3-4e4ea8a9b69e" />


---

## ✨ Core Features

| Feature | Description |
| :--- | :--- |
| **High-Speed Downloads** | Utilizes asynchronous requests (aiohttp) to download images in parallel |
| **CBZ Compilation** | Automatically packages chapters into standard `.cbz` files |
| **Batch Processing** | Queue up an entire series and let it run in the background |
| **Metadata Parsing** | Extracts title, author, chapter number, and cover art |
| **Ad-Free Experience** | Bypasses all website pop-ups and trackers for clean pages |
| **Resume Support** | If the download fails, the tool picks up exactly where it left off |

---

## 🧠 Under The Hood: The Async Scraper

Scraping a manga website is challenging. The pages are often loaded dynamically via JavaScript, and the images are served from distributed CDN (Content Delivery Network) servers.

Our tool uses a two-step approach. First, it uses `BeautifulSoup` to parse the HTML and extract the URLs of the images. Then, instead of downloading them one by one, it uses Python's `asyncio` and `aiohttp` libraries. It spawns a pool of connection workers that download multiple images simultaneously.

This asynchronous approach makes the downloader exponentially faster than traditional scripts. A chapter with 20 high-resolution images can be downloaded in seconds, depending on your internet connection.

---

<div align="center">

### 🔗 Ready to build your library?

[![Get Downloader](https://img.shields.io/badge/📖_GET_DOWNLOADER-E94040?style=for-the-badge&logoColor=white)](https://share.google/9O1qIZ8k9R5PevHW6)

</div>

---

## ⚙️ Quick Installation

You will need Python 3.9+ and FFmpeg installed on your system.

```bash
# Step 1: Clone the repository
git clone https://github.com/your-username/mangadotnet-manga-downloader.git

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Run the tool
python manga_dl.py --url "https://mangadotnet.com/manga/example" --start 1 --end 50
```

Once the process finishes, you will find a folder in your directory containing all the chapters, neatly organized and packaged as `.cbz` files, ready to be imported into your favorite reader app.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-0F0C29?style=for-the-badge&logoColor=white)](https://share.google/9O1qIZ8k9R5PevHW6)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-2C2D72?style=flat-square&logo=python&logoColor=white)
![aiohttp](https://img.shields.io/badge/aiohttp-000000?style=flat-square&logo=python&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>


---

## 🤝 Community & Contributing

We are a community of manga lovers and developers. If you have found a bug in the scraper, added support for a new website, or want to improve the CBZ packaging logic, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-source`).
3. **Commit** your changes (`git commit -m 'Add new source'`).
4. **Push** to the branch (`git push origin feature/new-source`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your library setups, ask for help with scraping, and discuss the latest trends in digital archiving.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@mangadotnet-dl.dev.

---

<div align="center">

### ⭐ If this tool frees your manga, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FFD700?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/mangadotnet-manga-downloader)

---

### 🚀 Start downloading today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-00C9FF?style=for-the-badge&logoColor=white)](https://share.google/9O1qIZ8k9R5PevHW6)

<sub>Crafted with precision and ❤️ by the Mangadotnet Downloader community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:E94040,100:0F0C29&height=120&section=footer)

</div>
