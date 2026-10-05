Masalah yang ditemukan adalah adanya aturan CSS yang saling bertabrakan pada selector `p` dan `.card p`, sehingga warna teks pada paragraf tidak mengikuti aturan yang diharapkan.

Contoh aturan CSS yang bertabrakan:

```css
p {
    color: green;
}

.card p {
    color: purple;
}
```

Penyebab

Selector `.card p` memiliki tingkat spesifisitas yang lebih tinggi daripada selector `p`, sehingga aturan `.card p` menjadi pemenang dalam cascade.

Perbaikan

Aturan CSS yang tidak diperlukan dihapus dan penggunaan selector disesuaikan. Setelah diperbaiki, tampilan teks kembali sesuai dengan sistem visual yang telah ditentukan.
