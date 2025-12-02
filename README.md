Quantum Recipe Book 🧪

Selamat datang di Quantum Recipe Book! Repositori ini adalah panduan visual dan analitis untuk memahami bagaimana gerbang kuantum memengaruhi keadaan sistem 3-qubit.
Setiap sirkuit adalah “resep”, dan setiap gerbang adalah “bahan” yang menciptakan “rasa” keadaan kuantum yang unik.


📖 Tujuan Proyek

Proyek ini bertujuan untuk:

Membuat dan memvisualisasikan sirkuit kuantum 3-qubit menggunakan Qiskit.

Menganalisis efek kumulatif dari gerbang dasar (H, X, Y, CX, CCX, Z, SWAP) pada vektor keadaan.

Memprediksi dan memvisualisasikan peluang pengukuran akhir.

🛠️ Bahan-Bahan dan Alat

Proyek ini dibangun menggunakan:

Bahasa Pemrograman: Python

Pustaka Kuantum: Qiskit (QuantumCircuit, Statevector, Aer, plot_histogram)

Lingkungan: Jupyter Notebook (quantum_magic.ipynb)

🍳 Resep Utama: Sirkuit Kuantum Ajaib
1. Adonan Awal (Superposisi)

Sistem dimulai dengan 3 qubit yang semuanya diberikan gerbang Hadamard (H) sehingga terbentuk superposisi penuh:

Keadaan awal: setiap dari 8 basis keadaan klasik memiliki peluang sama.

2. Proses Pencampuran (Gerbang Kuantum)

Urutan gerbang yang diterapkan pada qubit q2, q1, q0:

Langkah	Gerbang	Qubit	Fungsi
Awal	H	q0, q1, q2	Membuat superposisi
2	X	q0	Pembalikan bit (NOT kuantum)
2	CX	q1 (kontrol) → q2 (target)	Membentuk entanglement
3	Y	q2	Pembalikan bit + fase
4	CCX (Toffoli)	q0, q1 (kontrol) → q2 (target)	Gerbang AND terkontrol
5	X	q0	Pembalikan bit
5	Y	q1	Pembalikan bit + fase
6	Z	q1	Pembalikan fase
7	SWAP	q0 ↔ q2	Pertukaran keadaan qubit
3. Sirkuit Lengkap

Ini adalah visualisasi sirkuit akhir yang siap diukur.
(Tambahkan gambar sirkuit jika ada)

📊 Hasil Akhir dan Analisis

Setelah semua operasi diterapkan, vektor keadaan akhir memiliki amplitudo sama besar (positif atau negatif) untuk seluruh 8 basis keadaan.

Peluang Pengukuran

Amplitudo yang sama besar menghasilkan probabilitas yang sama pula.

Probabilitas untuk setiap hasil 000 hingga 111 adalah:

Probabilitas: 1/8

Persentase: 12.5%

Kesimpulan:
Meski ada fase negatif yang dihasilkan oleh gerbang seperti Y, Z, dan CCX, fase tersebut tidak memengaruhi probabilitas akhir.
Sistem tetap menghasilkan distribusi peluang yang seimbang untuk semua keadaan.

📉 Visualisasi Histogram


Histogram yang rata menunjukkan bahwa sirkuit ini menghasilkan keadaan yang merata pada semua basis.
