# 🇮🇱 Israel Skyline Live

A simple GitHub Pages website that displays **live skyline webcams from Israel** using embedded YouTube streams.

The project is designed so that **all streams are configured in a JSON file**, meaning you can add or remove cameras **without editing the HTML**.

---

# ✨ Features

* 📺 Multiple YouTube live streams on one page
* 🧩 Streams configured via `lives.json`
* 🔍 Built-in search (city / name / tag)
* ▶️ Toggle autoplay
* 📱 Fully responsive UI (works on phones and desktop)
* 🚀 Runs on **GitHub Pages (no server required)**

---

# 📂 Project Structure

```
/
├── index.html      # Main website UI
├── lives.json      # List of live streams
└── README.md
```

---

# ➕ Adding a New Live Camera

To add a camera, **edit `lives.json` only**.

Example:

```json
{
  "id": "tel-aviv",
  "name": "Tel Aviv Skyline",
  "city": "Tel Aviv",
  "youtubeId": "fIurYTprwzg",
  "tags": ["skyline", "city"],
  "enabled": true
}
```

Add it to the `"cards"` array.

Example full structure:

```json
{
  "title": "🇮🇱 Israel Skyline Live",
  "subtitle": "Live webcams via YouTube",
  "cards": [
    {
      "id": "tel-aviv",
      "name": "Tel Aviv Skyline",
      "city": "Tel Aviv",
      "youtubeId": "fIurYTprwzg",
      "tags": ["skyline"],
      "enabled": true
    }
  ]
}
```

---

# 🎥 What is a YouTube Video ID?

Every YouTube video or live stream has a **unique ID**.

Example:

```
https://www.youtube.com/live/fIurYTprwzg
```

The **video ID** is:

```
fIurYTprwzg
```

This is the value used in `youtubeId`.

---

# 🚀 Deploying to GitHub Pages

1. Create a GitHub repository
2. Upload:

```
index.html
lives.json
README.md
```

3. Go to:

```
Settings → Pages
```

4. Select:

```
Deploy from branch
Branch: main
Folder: /root
```

After deployment your site will appear at:

```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME
```

---

# ⚠️ Notes

* YouTube streams usually have a **5–30 second delay**.
* Some streams **disable embedding**, which means they will not load.
* The site is **static**, so it runs entirely on GitHub Pages.

---

# 📌 Future Improvements (Ideas)

* Auto-detect live streams from YouTube channels
* Map view of cameras
* Time-of-day labels (day/night)
* Optional alert overlay

---

# 🛠 Built With

* HTML
* CSS
* JavaScript
* GitHub Pages
* YouTube Embed API

---

# 📄 License

Only with permission by the creator, tripelsoda.
