#### **PAKET BAHASA AUSTRONESIA**

Terjemahan Bahasa Indonesia, Melayu, dan Filipina

Lokalisasi Asli Tanpa Sensor dengan Nuansa Budaya

[Halaman Subtitle THE WITCHER 3](https://karyain.net/game?slug=witcher3) · [![Watermark](https://img.shields.io/badge/Watermark-2.8%25-red)](#status--informasi-watermark)

***

##### Cara Pasang

1. Ekstrak berkas mod yang telah diunduh.
2. Salin isi dari folder bahasa ke dalam direktori instalasi game Anda.
3. Jalankan game dan nikmati!

***

##### Pelaporan Bug

Memeriksa kecocokan subtitle satu demi satu membutuhkan waktu yang sangat lama, karena prosesnya mengharuskan permainan dimainkan dari awal hingga akhir — bagaikan mencari jarum dalam tumpukan jerami. Jika Anda menemukan teks yang tidak biasa, kurang tepat, atau mengalami kendala teknis, mohon kirimkan tautan berkas simpanan game (*save game*), tangkapan layar (*screenshot*), serta bagian kalimat spesifik yang bermasalah. Umpan balik Anda sangat membantu proses perbaikan mod ini!

***

##### Kebijakan Penggunaan

Mod ini bukan merupakan hasil terjemahan instan menggunakan Google Translate atau ChatGPT yang disalin secara langsung. Mod ini adalah implementasi eksperimental dari alur penerjemahan saraf (*neural translation pipeline*) 8-fase yang sekitar 85% prosesnya berjalan secara luring (*offline*). Sistem ini saya rancang secara khusus untuk rumpun bahasa Austronesia, dan dibangun selama lebih dari 1500 jam sebagai bagian dari riset makalah akademis yang membutuhkan dedikasi tinggi. Anda dapat memeriksa detail alur (*pipeline*) tersebut secara langsung di situs web saya.

Agar alur penerjemahan dapat memproses ratusan ribu baris dialog tanpa membebani kinerja komputer secara berlebihan, eksperimen ini menggunakan:

*   **Custom Foundation Model:** Model AI yang saya latih ulang secara mandiri agar dapat memahami tiga bahasa sekaligus.
*   **Register-Adaptive LoRA:** Modul penyesuaian halus (*fine-tuning*) yang dapat beralih antara ragam bahasa formal, santai (kasual), dan netral — sehingga setiap karakter memiliki gaya bicara khas mereka masing-masing.
*   **Semantic Validation:** Alur pemrosesan bahasa alami (*NLP pipeline*) kustom untuk memvalidasi apakah hasil terjemahan secara semantik tetap selaras dengan makna aslinya.

***

##### Status & Informasi Watermark

**Status: Versi Eksperimental**

Karena alur penerjemahan yang sangat kompleks, Anda pasti akan menemukan beberapa bagian terjemahan yang kurang tepat, tag yang hilang, atau kalimat yang ambigu. Berhubung keterbatasan waktu untuk menyelesaikan permainan ini secara mandiri (saya hanya sempat memeriksa bagian awal permainan), umpan balik (*feedback*) dari Anda sekalian sangat krusial untuk proses pengembangan model. Upaya penulisan lebih dari 50 ribu baris kode ini melibatkan siklus berkelanjutan dari perancangan, pengujian, perbaikan kesalahan, hingga penyelarasan model.

**Watermark**

Ya, pada versi eksperimental ini terdapat **watermark sebesar 2.8%** yang tersisip langsung di dalam subtitle terjemahan. Sebagai catatan, sebagian kecil dari persentase watermark tersebut mungkin sedikit mengganggu kenyamanan visual, tetapi permainan tetap dapat dinikmati dengan baik.

Jika menginginkan versi tanpa watermark yang telah diterjemahkan sepenuhnya, Anda dapat mengunduhnya melalui [Trakteer](https://trakteer.id/skripsimu.myid/) atau [Ko-fi](https://ko-fi.com/skripsimumyid). Watermark **merupakan instrumen teknis yang sengaja diintegrasikan.** Fungsinya adalah untuk melacak distribusi dataset yang tidak biasa, membandingkan gaya bahasa, memantau hasil model (sebagai catatan, saya pun menggunakan versi dengan watermark), serta mencegah data yang belum matang disebarluaskan di luar ekosistem pengujian atau diklaim secara sepihak oleh pihak lain tanpa izin.

Watermark ini akan tetap dipertahankan hingga alur penerjemahan benar-benar stabil. Jika tidak ada watermark, berarti proyek ini tidak lagi dipelihara secara aktif. Keberadaan watermark menandakan bahwa Anda dapat mengharapkan pembaruan berkala karena proyek ini masih terus dikembangkan secara aktif.

**Umpan Balik**

Setiap masukan mengenai kualitas terjemahan sangat kami harapkan. Namun, jika keluhan hanya terkait keberadaan watermark, mohon maaf jika kami kurang responsif karena sudah dijelaskan sebelumnya bahwa persentase watermark akan terus berkurang pada setiap pembaruan.

***

##### Opsi yang Tersedia

1. **Terima Apa Adanya:** Mengunduh versi ini, memaklumi keberadaan watermark serta bug eksperimental, dan mencoba menikmati permainan.
2. **Bantu Menyempurnakan:** Mengirimkan tangkapan layar terjemahan yang bermasalah ke kolom komentar atau memberikan kritik konstruktif. Semua umpan balik Anda akan masuk ke sistem peninjauan manual (*Human Review Gate*) untuk pelatihan ulang model. Semakin banyak data yang terkumpul, semakin cepat versi tanpa watermark dapat dirilis.
3. **Dapatkan Versi Alpha Tanpa Watermark:** Berikan dukungan melalui [Trakteer](https://trakteer.id/skripsimu.myid/) atau [Ko-fi](https://ko-fi.com/skripsimumyid) untuk mendapatkan akses langsung ke versi pengembangan alpha tanpa watermark untuk mod ini dan berbagai proyek eksperimental lainnya. Kontributor yang memberikan dukungan biasanya memberikan masukan yang paling kritis dan mendalam.
4. **Lewati Saja:** Jika keberadaan watermark menjadi kendala utama dan Anda tidak ingin menggunakan versi uji coba ini, tidak menjadi masalah. Anda dapat menunggu versi stabil, menggunakan mod alternatif lain, atau menikmati permainan dalam bahasa aslinya.
   *Terima kasih atas pengertiannya, dukungan Anda sangat berarti bagi kelancaran riset akademis saya!*

***

##### Model yang Digunakan

Model AI berikut digunakan untuk menjalankan alur penerjemahan ini, seluruhnya dikonversi dan dijalankan menggunakan **ONNX Runtime**:

| Model | Fungsi |
|---|---|
| [t5gemma-2-1b-1b](https://huggingface.co/google/t5gemma-2-1b-1b) | Summarizer |
| [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | Clustering \& Klasifikasi |
| [gliner\_multi-v2.1](https://huggingface.co/urchade/gliner_multi-v2.1) | Named Entity Recognition (NER) |
| [multilingual-e5-large-instruct](https://huggingface.co/intfloat/multilingual-e5-large-instruct) | Bitext Mining / Kemiripan Semantik |
| [gemma-3-27b-it](https://huggingface.co/google/gemma-3-27b-it) | Penerjemah *(Sudah di fine-tuned secara agresif)* |

Seluruh model telah dikonversi ke format ONNX untuk proses inferensi berbasis GPU AMD pada sistem operasi Windows. (Tidak open-source.)

***

[Austronesian Lang Pack](https://karyain.net/)  ·  [Trakteer](https://trakteer.id/skripsimu.myid/rewards)  ·  [Ko-fi](https://ko-fi.com/skripsimumyid/shop)  ·  [Discord](https://discord.gg/REaQdcVepg)  ·  [YouTube](https://www.youtube.com/@arsip_skripsimu)
