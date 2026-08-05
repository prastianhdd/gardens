# 🌱 Gardens

Repository dengan auto-commit workflow yang kreatif menggunakan GitHub Actions!

## ✨ Fitur

| Fitur | Deskripsi |
|-------|-----------|
| 🔄 **Auto Commit** | Commit otomatis setiap 4 jam |
| 💬 **Pesan Random** | 30+ pesan kreatif yang berbeda-beda |
| 📊 **Statistik** | Tracking jumlah commit dan info lainnya |
| 🎨 **Emoji Random** | Emoji unik di setiap commit |
| 🎯 **Topik Random** | Topik acak di setiap commit |
| 📅 **Info Waktu** | Hari dan waktu dalam Bahasa Indonesia |
| 💡 **Fun Facts** | Fakta menarik tentang programming |

## 🎮 Cara Kerja

```
Setiap 4 jam:
┌─────────────────────────────────────┐
│  🔄 Trigger Workflow                │
│  ↓                                  │
│  🎨 Generate Random Content         │
│     - 30+ pesan kreatif             │
│     - 20 emoji random               │
│     - 10 topik random               │
│  ↓                                  │
│  📊 Update Statistik                │
│     - Commit count                  │
│     - Fun facts                     │
│  ↓                                  │
│  💾 Commit & Push                   │
│     - Pesan unik & kreatif          │
│     - Info lengkap di badan commit  │
└─────────────────────────────────────┘
```

## 📝 Contoh Commit Message

```
🚀 Lagi naik roket nih, commit tanpa henti!

⏰ Waktu: 2024-01-15 08:00:00 UTC
📅 Hari: Senin Pagi
🎯 Topik: Tentang teknologi
📊 Commit ke-42

_Auto committed by @prastianhdd_ 🤖
```

## 🚀 Cara Pakai

### 1. Push ke GitHub

```bash
git add .
git commit -m "🌱 Initial commit"
git remote add origin https://github.com/prastianhdd/gardens.git
git push -u origin main
```

### 2. Auto Commit Berjalan Sendiri

Workflow akan otomatis jalan setiap 4 jam!

### 3. Manual Trigger

1. Buka tab **Actions** di repository
2. Pilih **🌱 Auto Commit**
3. Klik **Run workflow**
4. Pilih branch → klik **Run workflow**

## 📊 Statistik

File statistik akan otomatis diupdate:

```
stats/
├── commit-count.txt    # Jumlah total commit
├── latest-commit.md    # Info commit terakhir
└── fun-facts.txt       # Kumpulan fun facts
```

## 🎨 Kustomisasi

### Tambah Pesan Baru

Edit array `MESSAGES` di `.github/workflows/auto-commit.yml`:

```bash
MESSAGES=(
  "pesan baru 1"
  "pesan baru 2"
  # ... tambah di sini
)
```

### Tambah Emoji

```bash
EMOJIS=("🆕" "🎉" "🎊")
```

### Tambah Topik

```bash
TOPICS=(
  "Tentang topik baru"
)
```

### Ubah Jadwal

Ganti cron expression:

```yaml
schedule:
  # Setiap jam (default: 4 jam)
  - cron: '0 * * * *'

  # Setiap hari jam 9 pagi
  - cron: '0 9 * * *'

  # Setiap 30 menit
  - cron: '*/30 * * * *'
```

## 📁 Struktur Repository

```
gardens/
├── .github/
│   └── workflows/
│       └── auto-commit.yml    # Workflow utama
├── stats/
│   ├── commit-count.txt       # Total commits
│   ├── latest-commit.md       # Info terakhir
│   └── fun-facts.txt          # Fun facts
├── .gitignore
└── README.md
```

## 🤖 Author

- **GitHub**: [@prastianhdd](https://github.com/prastianhdd)
- **Email**: prastianhd@gmail.com

---

_Dibuat dengan ❤️ oleh @prastianhdd_
