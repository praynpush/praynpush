# Pray&Push Personal Blog

Welcome to the official repository of **Pray&Push**, a personal blog focused on health, longevity, and lifestyle.

## 🚀 Modern Features

This blog is built on a highly customized version of the [Hugo Stack](https://github.com/CaiJimmy/hugo-theme-stack) theme, with several exclusive enhancements:

### 🎙️ Automatic Edge TTS (Podcast Mode)
Every blog post is automatically converted into high-quality audio using **Microsoft Edge TTS (Xiaoxiao Neural)**. 
- **How it works**: A GitHub Action triggers on every push, runs a Python script to generate the audio, and embeds a premium audio player directly into the article.
- **Listen while you read**: No need to download anything; just click play at the top of any post.

### 🎥 Lite YouTube Embeds
We've implemented a custom "Click-to-Play" YouTube component for article covers.
- **Performance**: Loads a lightweight image overlay first, preserving page speed.
- **Seamless**: Replaces the cover image with an auto-playing video only when clicked.

### 📱 Fully Responsive & Optimized
- Optimized OpenGraph and Twitter Cards for social media sharing.
- High-performance image processing using Hugo's built-in tools.

## 🛠️ Development

### Prerequisites
- [Hugo Extended](https://gohugo.io/installation/) (v0.160+)
- [Git](https://git-scm.com/)

### Local Setup
```bash
# Clone the repository
git clone --recursive https://github.com/praynpush/praynpush.github.io.git

# Start local development server
hugo server --disableFastRender
```

## 🏗️ Deployment
The site is automatically deployed to **GitHub Pages** via GitHub Actions whenever changes are pushed to the `master` branch.

## 📂 Project Structure
- `content/blog/`: Markdown source for blog posts.
- `themes/hugo-theme-stack/`: Our customized fork of the Stack theme.
- `scripts/`: Automation scripts (e.g., TTS generation).
- `.github/workflows/`: CI/CD pipelines for TTS generation and site deployment.

---
© 2026 **Pray&Push**. Built with ❤️ and Hugo.
