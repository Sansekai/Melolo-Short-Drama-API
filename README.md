# 🎬 Melolo Short Drama API

**Melolo Short Drama API** adalah layanan API gratis yang menyediakan akses ke berbagai konten drama pendek dan video shorts. API ini memungkinkan pengembang untuk mengambil data konten terbaru, trending, melakukan pencarian, melihat detail drama, hingga mendapatkan link streaming video.

<div align="center">
  <img src="https://github.com/Sansekai/Melolo-Short-Drama-API/blob/main/melolo.gif?raw=true" alt="Demo API" style="width:50%;">
</div>

---

## 🚀 Base URL

Semua request ditujukan ke host berikut:
[https://melolo-api-azure.vercel.app](https://melolo-api-azure.vercel.app)

## 📚 Daftar Endpoint

Berikut adalah daftar endpoint yang tersedia untuk layanan **Melolo**:

| Judul | Method | Endpoint | Deskripsi |
| :--- | :---: | :--- | :--- |
| **Konten Terbaru** | `GET` | `/melolo/latest` | Mengambil daftar konten drama/shorts terbaru. |
| **Konten Trending** | `GET` | `/melolo/trending` | Mengambil daftar konten yang sedang tren. |
| **Cari Konten** | `GET` | `/melolo/search` | Mencari konten berdasarkan kata kunci tertentu. |
| **Detail Konten** | `GET` | `/melolo/detail/:book_id` | Mengambil detail lengkap dari sebuah serial drama. |
| **Link Streaming** | `GET` | `/melolo/stream/:vid_id` | Mengambil link streaming untuk video/episode tertentu. |

-----

## 🛠️ Detail Parameter

### 🔍 Search (`/melolo/search`)

| Parameter | Tipe | Wajib? | Deskripsi |
| :--- | :--- | :---: | :--- |
| `query` | String | **Ya** | Kata kunci pencarian (contoh: `pewaris`). |
| `limit` | Number | Tidak | Jumlah hasil yang ditampilkan (Default: `10`). |
| `offset` | Number | Tidak | Offset untuk pagination (Default: `0`). |

### 📖 Detail & Stream

  * **`:book_id`**: ID unik dari drama didapatkan dari properti **`book_id`** (bisa didapatkan dari endpoint latest, search, & trending).
  * **`:vid_id`**: ID unik dari episode/video didapatkan dari properti **`vid`** (didapatkan dari endpoint detail).

-----

## 💼 Pembelian Source Code

Anda tertarik untuk memiliki source code lengkap dari API ini?

Silakan klik link pembelian:
**[Beli Source Code](https://lynk.id/sansekai/ygd0z9jowrlr)**

-----
