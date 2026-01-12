
Praktikum 7: Menerapkan Desain UI Modern
Proyek ini merupakan bagian dari mata kuliah Mobile Programming 20251. Fokus utama praktikum ini adalah mengimplementasikan prinsip desain modern menggunakan Material Design 3 (MD3), sistem tema yang modular, dan komponen UI yang dapat digunakan kembali (reusable) pada Android Studio dengan Jetpack Compose.
🎯 Tujuan Praktikum
 * Memahami dan menerapkan prinsip desain UI modern sesuai standar Material Design 3.
 * Mengimplementasikan sistem tema yang terdiri dari skema warna (color scheme), tipografi, dan bentuk (shape).
 * Membuat komponen UI yang modular dan konsisten.
 * Menerapkan fitur Dark Mode, Light Mode, dan Dynamic Color.
 * Membangun alur navigasi antar layar (Login, Register, Dashboard, Details, dan Settings).
🛠️ Struktur Proyek
Struktur folder diatur sedemikian rupa untuk menjaga kerapian dan kemudahan pemeliharaan kode:
id.antasari.p7_modern_ui_nimanda/
├── ui/
│   ├── theme/           # Konfigurasi Tema Global
│   │   ├── Color.kt     # Definisi palet warna (Primary, Secondary, dll)
│   │   ├── Type.kt      # Hierarki tipografi (Headline, Body, Label)
│   │   ├── Shape.kt     # Definisi sudut lengkung (Rounded corners)
│   │   └── Theme.kt     # Penggabungan elemen tema & logika Dark/Dynamic Mode
│   ├── components/      # Komponen UI Reusable
│   │   ├── AppButton.kt     # Primary & Secondary Outline Buttons
│   │   ├── AppTextField.kt  # Input teks dengan ikon & mode password
│   │   ├── AppCard.kt       # Container kartu dengan elevasi lembut
│   │   ├── SectionHeader.kt # Judul bagian dengan aksi opsional
│   │   └── TopBar.kt        # Center-aligned Top App Bar
│   └── screens/         # Implementasi Halaman Aplikasi
│       ├── LoginScreen.kt
│       ├── CreateAccountScreen.kt
│       ├── HomeScreen.kt
│       ├── SecurityDetailsScreen.kt
│       └── SettingsScreen.kt
└── MainActivity.kt      # Entry point & Logika Navigasi Sederhana

🚀 Fitur Utama
 * Design System Mini: Satu sumber kebenaran untuk warna, font, dan bentuk agar tampilan aplikasi seragam di seluruh layar.
 * Modern Login & Register: Form input lengkap dengan validasi visual, toggle show/hide password, dan opsi biometric login.
 * Interactive Dashboard: Menampilkan ringkasan keamanan, kartu aksi cepat (quick actions), dan riwayat aktivitas terbaru.
 * Adaptive Theme: Mendukung perpindahan otomatis antara tema terang dan gelap, serta warna dinamis pada perangkat Android 12+.
 * Security Settings: Halaman pengaturan yang fungsional dengan komponen Switch untuk mengelola notifikasi dan keamanan.
📝 Langkah Instalasi
 * Pastikan Anda menggunakan Android Studio versi terbaru.
 * Gunakan Minimum SDK: API 24 (Android 7.0).
 * Tambahkan dependensi Material 3 pada file build.gradle:
   implementation("androidx.compose.material3:material3:1.2.1")

 * Lakukan Sync Project with Gradle Files.
🎓 Penulis
 * Dosen Pengampu: Muhayat, M.IT
 * Topik: Material Design 3, Style, Theme, & Modern UI Principles
Dibuat berdasarkan Modul Praktikum MP #7 - 20251.
