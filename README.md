# Praktikum 2 - CSS Dasar

## Tujuan
1. Memahami konsep dasar CSS
2. Memahami aturan penulisan CSS
3. Memahami selector (element, class, id)
4. Mengimplementasikan CSS pada HTML

## Langkah Praktikum

### 1. Membuat Dokumen HTML
File: `lab2_css_dasar.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>

  <!-- CSS Internal -->
  <style>
    body {
      font-family: 'Open Sans', sans-serif;
      background-color: #f5f5f5;
    }
    header {
      min-height: 80px;
      border-bottom: 1px solid #77CCEF;
    }
    h1 {
      font-size: 24px;
      color: #0F189F;
      text-align: center;
      padding: 20px 10px;
    }
    h1 i {
      color: #6d6a6b;
    }
  </style>

  <!-- CSS Eksternal -->
  <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>

  <nav>
    <a href="lab2_css_dasar.html" class="active">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>

  <!-- ID Selector -->
  <div id="intro">
    <h1>Hello World</h1>
    <p style="text-align:center; color:#070b0f;"> <!-- Inline CSS -->
      Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di 
      <i>Universitas Pelita Bangsa</i>. Pelajaran pertama adalah membuat tampilan web sederhana.
    </p>
    <!-- Class Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
  </div>
</body>
</html>
```

## Jawaban Pertanyaan
1. Sudah diuji coba dengan menambah properti CSS (warna, font, spacing).  
2. `h1 {...}` berlaku untuk semua h1, sedangkan `#intro h1 {...}` hanya untuk h1 di dalam #intro.  
3. Inline CSS paling tinggi prioritasnya dibanding internal dan eksternal.  
4. Jika elemen punya ID dan Class, CSS ID akan menang (lebih spesifik).  

---

## Dokumentasi
(Sertakan screenshot hasil percobaan di browser)
