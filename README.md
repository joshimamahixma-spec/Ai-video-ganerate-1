# 🎬 OmniVid AI Studio - Platform Video AI Ultimate
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Deskripsi

**OmniVid AI Studio** adalah platform web premium untuk membuat video AI berkualitas tinggi dengan teknologi terdepan. Platform ini memungkinkan pengguna untuk mengubah ide, teks, URL, atau PDF menjadi video profesional dalam hitungan detik.

### ✨ Fitur Unggulan

- 🎯 **AI Video Generator** - Konversi teks/URL/PDF menjadi video 4K
- 🎨 **Pro Video Editor** - Timeline editing profesional dengan AI tools
- 📤 **Smart Export** - Multi-platform publishing (YouTube, TikTok, Instagram)
- 🤖 **AI Assistant** - Konsultan kreatif real-time
- 🎤 **Voice Clone AI** - Sintesis suara natural dengan berbagai pilihan voice
- 📊 **Dashboard Analytics** - Tracking performa video dan engagement
- 🔒 **Auto-Backup Cloud** - Penyimpanan aman di Google Drive

---

## 🚀 Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/joshimamahixma-spec/Ai-video-ganerate-1.git
cd Ai-video-ganerate-1
```

### 2. Buka di Browser
```bash
# Cukup buka file index.html di browser Anda
# atau gunakan Live Server (VS Code Extension)
```

### 3. Akses Platform
Buka `http://localhost:5500` (jika menggunakan Live Server)

---

## 📁 Struktur File

```
Ai-video-ganerate-1/
├── index.html           # Main application (All-in-One)
├── README.md            # Dokumentasi
└── .gitignore           # Git ignore rules
```

### Catatan Struktur
Platform ini dibangun sebagai **Single Page Application (SPA)** dengan:
- **Frontend**: HTML5 + Tailwind CSS + JavaScript Vanilla
- **Icons**: Phosphor Icons
- **Styling**: Tailwind CSS via CDN
- **No Backend Dependencies** - Siap untuk diintegrasikan dengan backend API

---

## 🎮 Panduan Penggunaan

### 1️⃣ **AI Video Generator** (View pertama)
- Input prompt atau paste link (YouTube, Article, TikTok)
- Pilih rasio video (9:16, 16:9, 1:1)
- Pilih AI Voice Clone (Ryan, Sarah, atau suara custom)
- Pilih visual style (Hyper-Realistic, Stock Footage, Motion Graphics)
- Klik **"Generate Video Auto-Magic"**
- Tunggu progress hingga selesai, otomatis masuk ke Editor

### 2️⃣ **Pro Video Editor** (View kedua)
- Timeline editing dengan multiple tracks (Text, Video, B-Roll, Audio)
- Drag-drop assets dari left panel
- AI Quality Metrics real-time (Viral Potential, SEO Score)
- Auto-Color, Watermark Removal, Subtitle Generation
- Preview player dengan playback controls
- Export ke Editor atau langsung ke Export

### 3️⃣ **Export & Publish** (View ketiga)
- Pilih resolusi (4K/2K/Full HD/8K)
- Format file (MP4/MOV/WEBM)
- Frame rate (24/30/60 FPS)
- Multi-destination storage (Device, Google Drive)
- Direct publishing ke:
  - YouTube Shorts
  - TikTok
  - Instagram Reels
  - Facebook
- Auto-optimize caption & hashtag per platform

---

## 🛠️ Teknologi & Dependencies

### Frontend Stack
```
- HTML5 - Semantic markup
- Tailwind CSS 3 - Utility-first CSS framework
- JavaScript (Vanilla) - No framework, pure JS
- Phosphor Icons - Modern icon library
```

### CDN Resources
```html
<!-- Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Inter..." rel="stylesheet">

<!-- Icons -->
<script src="https://unpkg.com/@phosphor-icons/web"></script>

<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>
```

---

## 💻 Development

### File Utama: `index.html`

Struktur HTML:
```
<body>
  ├── <aside> SIDEBAR (Navigation + Status)
  ├── <main>
  │   ├── <section id="generator-view"> Generator
  │   ├── <section id="editor-view"> Pro Editor
  │   ├── <section id="export-view"> Export & Publish
  │   └── ... (Other placeholder views)
  ├── <div id="ai-chat-widget"> Floating AI Chat
  └── <script> JavaScript Logic
</body>
```

### JavaScript Functions

#### Tab Navigation
```javascript
// Event listener untuk nav buttons
document.querySelectorAll('.nav-btn').forEach(btn => {
  btn.addEventListener('click', () => {
    // Switch views dengan fade animation
  });
});
```

#### AI Generator Simulation
```javascript
function startGeneration() {
  // Progress bar animation
  // Steps tracking (Script, Voice, B-Roll, Render, Subtitle)
  // Auto-switch ke Editor saat selesai
}
```

#### Chat Widget Toggle
```javascript
function toggleChat() {
  // Toggle visibility dengan scale animation
}
```

---

## 🎨 Color Scheme & Design

### Primary Colors
- **Primary**: Indigo-600 (`#4f46e5`)
- **Secondary**: Purple-600 (`#9333ea`)
- **Accent**: Yellow-400 (`#facc15`)

### Backgrounds
- **Main BG**: Slate-950 (`#03071a`)
- **Sidebar**: Slate-900 (`#0f172a`)
- **Cards**: Slate-800 (`#1e293b`)

### Animations
- Smooth transitions (0.3s - 0.5s)
- Pulse glow effect untuk AI elements
- Shine effect pada buttons
- Fade in/out untuk view switching

---

## 📱 Responsive Design

Platform fully responsive:
- **Desktop**: Full layout dengan sidebar
- **Tablet**: Optimized grid & panels
- **Mobile**: Stacked layout (dapat ditambahkan dengan media queries)

---

## 🔮 Roadmap & Future Features

- [ ] Backend API Integration (Node.js/Python)
- [ ] Real AI Video Generation (Stable Diffusion, OpenAI)
- [ ] User Authentication & Database
- [ ] Project Management System
- [ ] Team Collaboration Features
- [ ] Advanced Analytics Dashboard
- [ ] Mobile App (React Native)
- [ ] Marketplace untuk Templates & Assets

---

## 🐛 Known Issues & Limitations

### Current Limitations (v1.0)
- 🔴 Generasi video masih simulasi (tidak real AI)
- 🔴 Tidak ada backend - data tidak tersimpan
- 🔴 Chat widget adalah demo chatbot
- 🟡 Mobile experience masih perlu optimasi
- 🟡 Beberapa menu item belum fully implemented

### Placeholder Modules
- Dashboard & Analytics
- AI Research Engine
- AI Voice & Subtitle (detail view)
- Smart Repurposing
- File & Auto-Backup

---

## 💡 Cara Integrasi dengan Backend API

### Contoh untuk Generator:
```javascript
// Ganti simulasi dengan API call
async function startGeneration() {
  const prompt = document.getElementById('prompt-input').value;
  
  const response = await fetch('/api/generate-video', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ prompt, voice: 'ryan', style: 'hyper-realistic' })
  });
  
  const data = await response.json();
  // Update UI dengan hasil video
}
```

---

## 📞 Support & Contact

- 📧 Email: joshimamahixma@gmail.com
- 🌐 GitHub: https://github.com/joshimamahixma-spec
- 💬 Issues: https://github.com/joshimamahixma-spec/Ai-video-ganerate-1/issues

---

## 📄 License

MIT License - Bebas digunakan untuk project komersial & non-komersial.

---

## 👨‍💻 Author

**Joshi Mamahixma**
- GitHub: [@joshimamahixma-spec](https://github.com/joshimamahixma-spec)
- Fokus: AI Video Generation, Web Development

---

## 🙏 Ucapan Terima Kasih

- Tailwind CSS Team
- Phosphor Icons
- Dan semua contributor yang membantu!

---

**Made with ❤️ by Joshi Mamahixma | Last Updated: June 2026**
