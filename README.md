# CV Digital — Muhammad Sadad

Website Curriculum Vitae (CV) digital berbasis HTML, CSS, GitHub, dan Docker.

## Fitur
- HTML5 semantik: `header`, `nav`, `main`, `section`, `article`, `footer`
- Heading hierarkis `h1`–`h3`, foto profil, navigasi antar bagian
- External CSS (`style.css`), layout Flexbox, CSS Grid untuk Skills & Portfolio
- Background profil, hover effect, tombol Download / Print CV (`window.print()`)
- Bagian: Tentang, Pendidikan, Pengalaman Kerja, Keahlian, Portofolio, Kontak

## Struktur Project
```
cv-digital/
├── index.html
├── style.css
├── profile.jpg
├── Dockerfile
└── README.md
```

## Menjalankan Tanpa Docker
Buka `index.html` di browser, atau:
```bash
python3 -m http.server 8080
# buka http://localhost:8080
```

## Menjalankan dengan Docker
```bash
docker build -t cv-digital .
docker run -d -p 8080:80 --name cv-digital cv-digital
docker ps
# buka http://localhost:8080
```

Untuk berhenti dan hapus container:
```bash
docker stop cv-digital
docker rm cv-digital
```

## Git & GitHub
Repository: `cv-digital`
```bash
git init
git add .
git commit -m "Initial commit: struktur HTML CV"
git commit -m "Tambah styling CSS dengan Flexbox dan Grid"
git commit -m "Tambah Dockerfile dan README"
git remote add origin https://github.com/bangdad/cv-digital.git
git branch -M main
git push -u origin main
```

## Catatan
Ganti data di `index.html` (nama, pendidikan, pengalaman, keahlian, portofolio, kontak) dan file `profile.jpg` dengan data asli Anda sebelum dikumpulkan.
