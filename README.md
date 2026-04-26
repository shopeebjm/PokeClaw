<img src="https://readme-typing-svg.herokuapp.com?color=%2336BCF7&center=true&vCenter=true&lines=TikTok+@shopee.bjm" />
</p>
<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?color=%2336BCF7&center=true&vCenter=true&lines=P+o+k+e+C+l+a+w" />
</p>

<h2 align="center">
  
[![Powered By:shopeebjm](https://img.shields.io/badge/PoweredBy:shopeebjm-7%2B-blue.svg?style=flat)](http://shopee.co.id/infinixnote40bjm)

<img src="https://img.shields.io/badge/Version-1.0.0-blue.svg"></h2>

</p>

<p align="center">
  <img src="banna.png" width="600" />
</p>
<p align="center">
  <img src="option.png" width="600" />
</p>

<p align="center">
  <a href="https://github.com/shopeebjm/PokeClaw/stargazers"><img src="https://img.shields.io/github/stars/shopeebjm/PokeClaw?style=social" alt="Stars" /></a>
  <a href="https://github.com/shopeebjm/PokeClaw/network/members"><img src="https://img.shields.io/github/forks/shopeebjm/PokeClaw?style=social" alt="Forks" /></a>
  <a href="https://github.com/shopeebjm/PokeClaw/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/shopeebjm/PokeClaw?style=social" alt="Closed Issues" /></a>
  <img src="https://img.shields.io/badge/Android-9%2B-3DDC84?logo=android&logoColor=white" alt="Android 9+" />
  <a href="https://github.com/shopeebjm/PokeClaw/releases/latest"><img src="https://img.shields.io/github/v/release/shopeebjm/PokeClaw" alt="Latest Release" /></a>
</p>

<p align="center">
  🌐 <a href="https://shopeebjm.github.com/PokeClaw/">Landing Page</a> — available in English · हिन्दी · 日本語 · Deutsch · 繁中
</p>

# PokeClaw (PocketClaw) — Agen Ai Di Perangkat Ponsel

`PokeClaw` juga dikenal sebagai `PocketClaw` adalah aplikasi Android sumber terbuka untuk otomatisasi ponsel berbasis AI.

Aplikasi ini dapat menjalankan Gemma 4 di perangkat untuk kontrol telepon lokal dan pribadi, dan juga mendukung model cloud opsional ketika Anda menginginkan penalaran yang lebih kuat untuk tugas-tugas yang lebih sulit.

Versi publik saat ini adalah prototipe yang mengutamakan lokal untuk mengubah ponsel Android menjadi perangkat yang dioperasikan oleh AI.

Dalam mode Lokal, eksekusi model tetap berada di dalam perangkat Anda. Tidak diperlukan akun atau kunci API untuk mode Lokal.



```
Everyone else:  Phone → Internet → Cloud API → Internet → Phone
                       💳Credit card needed, API key required. Monthly bill attached.

PokeClaw local: Phone → LLM → Phone
                       Local-first when you want it. Optional cloud when you need it.
```
**AI dapat mengontrol ponsel Anda, dengan eksekusi lokal terlebih dahulu dan bantuan cloud opsional.**

Versi publik saat ini bersifat open-source dan sudah menangani alur obrolan, tugas, dan otomatisasi yang sebenarnya di Android.

Pantau kontak WhatsApp dan balas otomatis:


Context-aware WhatsApp auto-reply:

https://github.com/user-attachments/assets/5a43d4d5-458a-4eea-a0a5-58d113255741

https://github.com/user-attachments/assets/5c2966c5-04e6-4b22-8d66-11915ae62096

> **☝️ Auto-reply demo:** PokeClaw memantau pesan dari Ibu, membaca apa yang dikatakannya, dan membalas berdasarkan konteks menggunakan LLM (Learning Language Memory) di perangkat. [Watch in higher resolution on YouTube](https://youtube.com/shorts/Vxpf474chm0)

> **☝️ Context demo:** Ibu bertanya "apa yang sudah Ibu suruh kamu bawa?" — AI membuka obrolan, membaca seluruh percakapan di layar, melihat pesan sebelumnya tentang anggur, dan membalas dengan benar. Inilah perbedaan antara balasan yang peka konteks dan balasan yang tidak peka konteks.

https://github.com/user-attachments/assets/89999dd8-a1be-49ad-9419-60c2b38f6374


> **Why is the "hi" demo slow?** Klip itu direkam pada perangkat Android yang hanya menggunakan CPU tanpa jalur GPU atau NPU yang dapat digunakan. Menjalankan Gemma 4 E2B pada CPU murni membutuhkan waktu sekitar 45 detik untuk pemanasan. Pada ponsel yang lebih canggih, prosesnya jauh lebih cepat:
> - **Google Tensor G3/G4** (Pixel 8, Pixel 9)
> - **Snapdragon 8 Gen 2/3** (Galaxy S24, OnePlus 12)
> - **Dimensity 9200/9300** (recent MediaTek flagships)
> - **Snapdragon 7+ Gen 2+** (mid-range with GPU)
>
> Pada perangkat ini, waktu pemanasan turun menjadi beberapa detik. Model yang sama, perangkat keras yang lebih baik.








## Cerita

Saya membangun ini sendirian. Ketika Gemma 4 hadir dengan pemanggilan alat bawaan pada LiteRT-LM, saya ingin tahu apakah ponsel dapat menjadi agen di perangkat yang sesungguhnya, bukan hanya sekadar chatbot. PokeClaw adalah hasilnya.

Bagian yang menarik bukanlah sekadar mengobrol dengan model lokal. Bagian yang menarik adalah membuat model lokal membaca layar, memilih alat, mengoperasikan aplikasi, menyimpan status tugas, dan menyelesaikan alur kerja ponsel yang sebenarnya. Itulah tepatnya tujuan dari proyek ini.

PokeClaw sudah mendukung otomatisasi sepenuhnya di perangkat dengan Gemma 4 dan model cloud opsional untuk eksekusi tugas yang lebih kuat. Fokus saat ini adalah dukungan perangkat yang lebih luas, keterampilan yang lebih umum, lebih banyak opsi model lokal, dan jalur rilis publik yang lebih bersih.

**Jika Anda menemukan sesuatu yang menarik,[buatlah sebuah issue](https://github.com/shopeebjm/PokeClaw/issues).** Laporan dari perangkat sebenarnya adalah cara agar hal ini dapat berkembang dengan cepat.

## Arah Produk

PokeClaw bukan sekadar aplikasi obrolan dengan beberapa trik kontrol ponsel yang ditambahkan di atasnya.

Pada intinya, ini menjadi sebuah **perangkat pendukung agen bergerak** :

lapisan alat generik untuk kontrol telepon
sebuah perulangan tugas/runtime yang memungkinkan model untuk memilih dan menghubungkan alat-alat tersebut.
Panduan, aturan, dan pengamanan yang dapat diuji coba terhadap pengujian kualitas perangkat nyata.
cangkang produk di bagian atas sehingga tali pengikat yang sama dapat digunakan oleh orang biasa, bukan hanya pengembang.
Perbedaan itu penting. Tujuan jangka panjangnya bukanlah untuk terus-menerus membuat alur aplikasi sekali pakai yang kaku. Tujuannya adalah untuk membangun kerangka kerja praktis terkuat untuk agen AI di ponsel Android, kemudian meluncurkan pengalaman produk di atas fondasi tersebut.

Itulah juga alasan mengapa proyek ini berinvestasi besar-besaran pada:

alat generik sebelum alur kerja yang lebih spesifik
Pengujian kualitas perangkat nyata yang berulang, bukan hanya demonstrasi sekali saja.
Perbandingan model Cloud vs Lokal pada kelompok tugas yang sama
Panduan dan aturan hanya digunakan ketika model tersebut terbukti membutuhkan struktur tambahan.

## Lihat UI

👉 **[Try the interactive demo on our landing page](https://shopeebjm.github.io/PokeClaw/)** — click through every screen without installing anything.

## Apa Fungsinya !

Model tersebut memilih alat yang tepat, mengisi parameter, dan mengeksekusi. Anda tidak perlu mengkonfigurasi apa pun untuk setiap aplikasi. Model tersebut hanya membaca layar dan bertindak.

## Tugas Cepat yang Terbukti

Ini adalah tugas-tugas yang telah kami jalankan secara menyeluruh selama pengujian kualitas (QA) di perangkat.

### Local mode

- Ringkaskan pemberitahuan
Jelaskan isi clipboard.
- Menganalisis penyimpanan/aplikasi dan menyarankan target pembersihan.
- Periksa apakah baterai perlu diisi daya.
- Laporkan aplikasi yang terpasang
- Laporkan suhu telepon
- Laporkan status Bluetooth
- Laporkan status baterai, penyimpanan,dan versi Android.
- Jalankan kartu tugas cepat langsung dari antarmuka pengguna dan kembalikan hasilnya di obrolan.
- Arahkan tugas kirim/panggilan khusus kontak dengan benar dan berikan penanganan kegagalan yang baik ketika kontak tidak ada di perangkat.

### Cloud mode

- Kirim pesan WhatsApp dan otomatis kembali ke percakapan PokeClaw yang sama.
- Cari di dalam YouTube di aplikasi sebenarnya.
- Periksa apa yang sedang tren di Twitter/X dan rangkumlah.
- Instal atau buka Telegram dari Play Store.
- Buka Reddit dan caripokeclaw
- Salin subjek email terbaru dan cari di Google.
- Buatlah draf email yang menyatakan bahwa Anda akan terlambat.
- Pertahankan status tugas dan riwayat sesi di seluruh eksekusi lintas aplikasi dan kembalikan

## Pengujian Kinerja & Jaminan Kualitas Perangkat Nyata

Setiap angka di bawah ini berasal dari uji coba berulang pada Pixel 8 Pro fisik yang menjalankan build rilis. Tidak ada uji coba yang dipilih-pilih, tidak ada emulator. Daftar tugas terverifikasi lengkap dan rincian tingkatannya ada di [thoughts/verified-task-capabilities.md](thoughts/verified-task-capabilities.md).

### Cloud (GPT-4.1) — 18/20 pass, real tasks on real phone

| Task | Result | Rounds | What happens |
|---|---:|---:|---|
| Search YouTube for lofi beats | ✅ | 9 | Opens YouTube, types query, hits search |
| Open Chrome and search for weather | ✅ | 9 | Opens Chrome, types query, reads results |
| Open Chrome and go to reddit.com | ✅ | 7 | URL navigation with node_id targeting |
| Compose email to test@example.com | ✅ | 12 | Opens Gmail, fills To + Subject + Body |
| Install Telegram from Play Store | ✅ | 14 | Search + tap Install + wait |
| Turn on do not disturb | ✅ | 12 | Navigates Settings, toggles DND |
| Open Settings, go to About Phone | ✅ | varies | Deep settings navigation |
| Send hi to Mom on WhatsApp | ✅ | 5 | Opens WhatsApp, finds contact, types, sends |
| Check my Instagram messages | ✅ | 5 | Handles typo ("instagarm"), opens correct app |
| 部機仲有幾多storage | ✅ | 2 | Cantonese input, returns answer in 中文 |
| 打開Instagram | ✅ | varies | Chinese command |
| Draft an email saying I'll be late | ✅ **10/10** | 8 | Repeated trials: 100% pass rate |
| Copy latest email subject and Google it | ✅ **8/10** | 15 | Gmail to Chrome cross-app flow, 80% pass rate |

Semua tugas tidak menggunakan logika aplikasi yang dikodekan secara manual. Model membaca layar, memilih alat, dan menentukan alurnya sendiri. Dukungan multibahasa berfungsi langsung tanpa perlu konfigurasi tambahan, termasuk bahasa Kanton, Mandarin, dan bahasa Inggris yang salah eja.

### Local (Gemma 4 E2B, fully on-device) — verified on CPU and GPU

| Task family | Result | CPU avg (Pixel 8 Pro) | GPU avg (Pixel 8 Pro) | Notes |
|---|---:|---:|---:|---|
| Clipboard explain | ✅ | 2m 43s | 2m 11s | Real clipboard read |
| Notifications summary | ✅ | 2m 49s | 2m 53s | Reads live notifications and summarizes |
| Battery advice | ✅ | 2m 12s | 2m 53s | Returns level + charging state |
| Storage + apps cleanup advice | ✅ | 2m 33s | 3m 06s | Harness used to mislabel this as blocked because the answer mentioned the Contacts app |

Untuk `local-core` paket tugas cepat saat ini pada Pixel 8 Pro, Gemma 4 E2B lolos pengujian `4/4` pada CPU dan GPU. Waktu rata-rata cold-start lebih banyak `2m 34s` pada CPU dibandingkan `2m 46s` pada GPU, jadi GPU sekarang **terverifikasi dan dapat digunakan** pada perangkat ini, tetapi **belum merupakan peningkatan kecepatan cold-start** untuk paket tugas singkat ini. Nilai dari pekerjaan pengerasan terbaru adalah stabilitas dan verifikasi backend yang sebenarnya, bukan sekadar pertunjukan benchmark yang dilebih-lebihkan.



# Cara Kerjanya
PokeClaw memberikan serangkaian alat kepada LLM (Live Link Manager) kecil di perangkat (ketuk, geser, ketik, buka aplikasi, kirim pesan, aktifkan balasan otomatis, dll.) dan membiarkannya memutuskan apa yang harus dilakukan. LLM melihat representasi teks dari layar saat ini, memilih tindakan, melihat hasilnya, memilih tindakan berikutnya, hingga tugas selesai.

Eksekusi lokal berjalan melalui LiteRT-LM dengan pemanggilan alat asli. Dalam mode Lokal, model berjalan di perangkat.

Local execution runs via [LiteRT-LM](https://ai.google.dev/edge/litert/llm/overview) with native tool calling. In Local mode, the model runs on-device.

## Peralatan

LLM memiliki akses ke alat-alat ini dan memilihnya secara mandiri:

| Tool | What it does |
|------|-------------|
| `tap` / `swipe` / `long_press` | Touch the screen |
| `input_text` | Type into any text field |
| `open_app` | Launch any installed app |
| `send_message` | Full messaging flow: open app, find contact, type, send |
| `auto_reply` | Monitor a contact and reply automatically using LLM |
| `get_screen_info` | Read current UI tree |
| `take_screenshot` | Capture screen |
| `finish` | Signal task completion |

Alat-alat ini bersifat umum — alat ini berfungsi dengan aplikasi apa pun, kontak apa pun, dan bahasa apa pun. LLM memilih alat yang tepat dan mengisi parameter dari permintaan Anda.

# Alat + Keterampilan
Model kecil di perangkat akan jauh lebih baik jika Anda memberinya panduan yang kuat. Oleh karena itu, kami memberikan PokeClaw kemampuan yang dapat digunakan kembali di samping alat-alat generik.

Fitur balasan otomatis adalah contoh yang bagus. Fitur ini tidak bekerja secara ajaib — ada alur kerja yang telah ditentukan sebelumnya di baliknya: buka obrolan → baca semua pesan yang terlihat di layar → buat balasan yang sesuai konteks → kirim → kembali ke halaman utama. Model ini mengikuti resep ini langkah demi langkah. Setiap alat dalam rantai tersebut bersifat umum: `open_app` berfungsi dengan aplikasi apa pun, `read_screen` berfungsi di layar apa pun,`send_message` berfungsi dengan kontak apa pun. Alur kerja hanya memberi tahu model alat mana yang harus digunakan dan dalam urutan apa.

Inilah yang kami sebut `Keterampilan` — alur kerja yang dapat digunakan kembali yang dibangun dari alat-alat generik. Kami secara aktif merancang sistem keterampilan yang terinspirasi oleh [arsitektur keterampilan Claude Code](https://docs.anthropic.com/en/docs/claude-code/skills). Idenya: siapa pun dapat menulis keterampilan sebagai file teks sederhana yang menjelaskan langkah-langkahnya, dan LLM mengikutinya.

Beberapa contoh hal yang dapat dilakukan oleh keterampilan:

`Balas otomatis` : pantau notifikasi → buka obrolan → baca percakapan → buat balasan → kirim
`Ringkasan pagi` : buka aplikasi cuaca → baca suhu → buka kalender → baca acara hari ini → buka email → hitung email yang belum dibaca → rangkum semuanya
`Penerusan cerdas` : tangkap notifikasi → buka pesan → baca → teruskan ke kontak lain dengan ringkasan.
`Pemesanan otomatis` : buka aplikasi pemesanan → cari slot waktu → isi detail → konfirmasi
Setiap keterampilan hanyalah kombinasi dari alat-alat umum yang sama ( `open_app`, `tap`, `type`, `read_screen`, `send_message`, dll.) yang disusun dalam urutan tertentu. Alat-alat tersebut adalah blok bangunan, keterampilan adalah resepnya.

Keduanya dirancang agar dapat diperluas. Kami membangun 8-10 keterampilan pertama sebagai fitur bawaan. Jika sistemnya berfungsi dengan baik, kami akan membukanya bagi komunitas untuk membuat dan berbagi alat dan keterampilan mereka sendiri. Anda lebih mengenal ponsel Anda daripada kami — Anda seharusnya dapat mengajarkan trik baru padanya.

Seiring model pada perangkat menjadi lebih pintar, sebagian besar hal ini dapat menjadi bebas bentuk. Saat ini, keterampilan adalah cara kita mendapatkan otomatisasi yang andal dari model lokal kecil sambil menjaga lapisan alat tetap generik.

## Download

[**Download APK**](https://github.com/shopeebjm/PokeClaw/releases/latest)

> Catatan: Jika Anda memperbarui dari versi debug publik yang lebih lama dan Android mengatakan paket tersebut tidak kompatibel, hapus instalasi versi lama sekali lalu instal APK terbaru dari awal. Versi debug publik yang lebih lama masih menerima pemberitahuan pembaruan dalam aplikasi, tetapi perlu diinstal ulang satu kali sebelum bergabung dengan 0.6.xjajaran versi stabil yang ditandatangani.

### Requirements

| | Minimum | Recommended |
|---|---|---|
| **Android** | 9+ | 12+ |
| **Architecture** | arm64 | arm64 |
| **RAM** | 8 GB | 12 GB+ |
| **Storage** | 3 GB free (model download) | 5 GB+ |
| **GPU** | Not required (CPU works) | Tensor G3/G4, Snapdragon 8 Gen 2+, Dimensity 9200+ |
| **Root** | Not required | Not required |

> ⚠️ 8 GB gets you in the door. 12 GB+ is the sweet spot for the built-in Gemma 4 local models, especially if you want smoother multitasking and faster model bring-up.

## Quick start

1. Install the APK
2. Grant Accessibility permission when prompted
3. If you want background monitor flows, also grant Notification Access
4. In Local mode, the model downloads on first local launch (~2.6 GB)
5. Switch to Chat or Task mode and start using it

Local mode needs no account and no API key. Cloud mode is optional.

## Roadmap

This is the current direction for PokeClaw based on real device testing, open issues, and the most common feature requests.

### Near-term

- **Stabler public releases and upgrades.** The release/signing path is being locked down so future public APKs upgrade cleanly instead of falling back to uninstall/reinstall behavior from the older debug-signed builds.
- **Missed-call auto follow-up.** A high-priority use case is: someone calls, you miss it, and PokeClaw automatically sends a follow-up message to that caller and keeps the status visible in the same chatroom. The preferred first path is SMS/API-first. WhatsApp follow-up is only worth adding if there is a reliable non-UI route; otherwise it should stay an explicit fallback path, not the core design.
- **Lower-RAM local model options.** Right now the built-in local model choices are still too heavy for a lot of mid-range phones. Smaller on-device models are high priority.
- **More small local models for real device coverage.** 1B–1.5B class models for lower-end phones are on the roadmap so more devices can at least run a usable local agent instead of being locked out by RAM limits.
- **More reliable local model downloads.** Resume/retry behavior, partial download cleanup, and corrupted-model detection are all being hardened so downloads survive weak connections and screen-off/resume cases better.
- **Broader device compatibility.** Samsung, Xiaomi, Dimensity, and low-RAM device issues are being used as real-world test cases for GPU→CPU fallback, model loading, accessibility reconnects, and generic UI control.
- **More generic phone-control skills.** We are continuing to replace brittle, app-specific assumptions with generic tools and reusable skills so tasks survive OEM UI changes better.

### In progress

- **Import your own local `.litertlm` models.** User-accessible local model import is on the roadmap so you can bring your own LiteRT model instead of being locked to the built-in download list.
- **Custom local model sources.** We want PokeClaw to go beyond a fixed built-in catalog and support user-defined model sources, including direct downloads from Hugging Face or other hosted URLs.
- **Google AI Core / system local AI integration.** We are tracking Android's newer on-device AI stack so PokeClaw can eventually use official system-level local model APIs where they make sense, instead of relying on a single runtime path forever.
- **More built-in workflows.** More quick-task / skill coverage is planned beyond the first WhatsApp-centric workflows.
- **Remote control / remote conversation flows.** Controlling a phone from another device is a real request and is on the longer roadmap, but it is not the current top priority compared with local reliability and device coverage.

### Known platform constraints

- **Edge Gallery model detection is not fully under our control.** Android hides other apps' `Android/data/...` sandboxes from normal file-pickers, so PokeClaw cannot generically "see" Edge Gallery's downloaded models unless they are exported into a user-accessible location first.
- **Sideload + accessibility apps may trigger OEM security warnings.** Samsung / Play Protect warnings are being addressed through a cleaner release/signing path, but sideload trust prompts are partly controlled by the platform and OEM policy.

### Where feature requests go

If you want something added, please open an issue. The roadmap above is intentionally built from real requests like:

- missed-call auto follow-up messages
- smaller local models for lower-end phones
- importing your own local models
- custom local model sources / hosted downloads
- Android AI Core / official on-device AI support
- cleaner upgrade/install paths
- remote control from another phone
- broader distribution paths like F-Droid

## Help Wanted

PokeClaw is moving fast, and the roadmap is being shaped directly by real device reports, feature requests, and QA results. If you want to help push local phone agents forward:

- ⭐ **[Star this repo](https://github.com/agents-io/PokeClaw)** if you think local AI phone control matters
- 🐛 **[Open an issue](https://github.com/agents-io/PokeClaw/issues)** when you hit a bug or want a feature
- 🍴 **[Fork it](https://github.com/agents-io/PokeClaw/fork)** and build on it

Every star helps more people find the project. Every issue helps shape the next release.

## Changelog

### v0.6.0 (2026-04-11)
- **Mainline release hardening.** Cloud and Local chat/task flows were tightened before release instead of shipping more speculative features on top.
- **Cloud task routing is less fragile.** Ordinary chat prompts like `say hi` no longer misroute into send-message behavior, while Cloud task flows still retain their multi-step capability.
- **Local chat continuity is materially better.** The on-device chat session now restores visible conversation history after session rebuilds and app relaunches, instead of silently losing the earlier turns.
- **Cloud and Local relaunch continuity are now verified.** Same-conversation memory survives a full force-stop/relaunch on both Cloud and Local paths.
- **Direct device-data tasks are more truthful.** Clipboard, notifications, battery, storage, and installed-app questions use the real device tools instead of generic chatbot refusals.
- **Models and settings are more honest.** The Models page now separates `Active model`, `Default local model`, and `Default cloud model`, and linked built-in Gemma rows no longer pretend the model is missing when the file is already usable.
- **Cloud model switching is cleaner.** Switching cloud models now emits one clear system line instead of duplicate switch messages.
- **Task/process UI is less noisy.** Normal chat no longer shows the orange `Task running...` bar, while true long-running work still shows the correct active state.
- **Local session ownership is hardened.** Chat-side local loading now stands down while a Local task owns the LiteRT session, preventing the old `session already exists` race.
- **Cloud release QA now uses success rate, not single-run theater.** The headline compose task passed `10/10`, and the Gmail-subject-to-Google exploratory task passed `8/10`, which is the right standard for stochastic Cloud flows.

### v0.5.1 (2026-04-10)
- **Chat/task input is more robust across phones.** The bottom input bar now follows the keyboard and system inset directly instead of relying on outer layout resize, which is safer across Pixel/Samsung navigation modes.
- **Public release signing is now pinned to a stable path.** GitHub releases now refuse to publish unless a stable signing key is configured, and the release workflow builds a signed `release` APK instead of accidentally shipping a debug artifact.
- **Release artifacts now include checksums.** The release pipeline also uploads `SHA256SUMS.txt` alongside the APK for easier verification.

### v0.5.0 (2026-04-10)
- **Previously shipped task flows now actually work.** Fixed stale model config reuse after switching Local/Cloud, fixed task/chat tab drift, fixed accessibility reconnect races, and fixed local task cancellation/session cleanup so tasks return to the right conversation instead of leaving stale state behind.
- **Previously broken task completions now execute the real app flow.** Explicit email-compose tasks now open a real mail composer instead of stopping with draft text in chat, and in-app search tasks can no longer fake-complete before the query is actually typed on screen.
- **Quick-task QA expanded.** Local quick tasks were swept end-to-end on-device, Cloud quick tasks now have cleaner automated coverage, and the QA runner correctly distinguishes real failures from environment blockers like permission dialogs or missing contacts.
- **Task budget default is now unlimited.** Fresh installs no longer inherit a fake default cap during development; users can still set a manual token/cost budget in Settings if they want one.
- **Previously misleading status rows now tell the truth.** Local GPU→CPU fallback now shows the real backend, the Accessibility status row reflects the real system state, and the Task Budget row shows `Unlimited` when no manual budget is set.
- **The updater now covers more real-world installs.** From v0.5.0 onward, accidental debug-build users also get the once-per-day GitHub release check, and the dialog warns when Android may require uninstalling an old debug build before installing the new APK.
- **Verified release-upgrade behavior.** Older public `0.4.0` builds do show the `v0.5.0` in-app update prompt, but upgrading from the old public debug signing path to the new public APK is a one-time uninstall + reinstall instead of an in-place replace.

<details>
<summary>Older versions (v0.1.0 — v0.4.1)</summary>

### v0.4.1 (2026-04-08)
- **Experimental task badge.** Task tab now shows `Experimental — more workflows coming soon`.
- **12 new complex task QA cases.** Added broader Cloud task coverage for YouTube search, contextual messaging, screen reading, settings toggles, app installs, web search, email compose, camera flows, typo tolerance, and ambiguous requests.

### v0.3.2 (2026-04-07)
- **Security fix.** Debug task receivers now disabled in release builds. External apps can no longer trigger tasks via broadcast.
- **Security fix.** The LAN config server was binding to all network interfaces, exposing API keys to anyone on the same WiFi. Now binds to localhost only.

### v0.3.0 (2026-04-07)
- **Cloud LLM support.** Chat and task modes now work with OpenAI, Anthropic, Google, and any OpenAI-compatible API. Switch providers with one tap in the new tabbed LLM Config screen.
- **Real-time token and cost display.** See your token count and running cost in the chat header as you talk. Color shifts from grey to blue to amber to red as usage climbs. No other mobile AI app shows you this.
- **Per-provider API keys.** Store a different API key for each provider. Switching tabs loads the right key automatically.
- **Mid-session model switch.** Start a conversation with GPT-4o, switch to Claude mid-chat, and keep your entire history. The new model picks up where the old one left off.
- **3-tier pipeline router.** Simple commands (call, alarm, open app) now execute instantly with zero LLM calls. Skill-matched tasks run deterministic step sequences. Only complex tasks hit the full agent loop.
- **8 built-in skills.** Search in App, Dismiss Popup, Scroll and Read, Send WhatsApp, Navigate to Tab, and more. Each skill saves 3-10 LLM rounds by running a hardcoded tool sequence instead of reasoning from scratch.
- **Skills UI in Task tab.** Quick Actions section shows all available skills with category icons. Tap to prefill the input bar.
- **Token budget system.** Set soft and hard limits on token usage per task. The floating pill shows live token count and cost, and you can tap to stop a runaway task.
- **Stuck detection.** Five signals detect when the agent is going in circles: repeated actions, unchanged screens, rising token count. Three-level recovery escalates from hints to strategy switches to auto-kill.
- **Enter and Tab key support.** Skills can now press Enter to submit search queries and Tab to move between form fields.

### v0.2.4 (2026-04-06)
- **Task tab redesigned with skill cards.** No more typing free-form commands that Gemma misunderstands. Two skill cards with fill-in-the-blank forms: "Monitor [name] on [WhatsApp]" and "Send [message] to [name] on [WhatsApp]".
- **Java skill routing.** Monitor and send-message tasks bypass the LLM entirely. Instant activation, zero warmup.
- **Progress bar on skill activation.** Card fills up and turns orange when active. You know exactly when monitoring starts.
- **Custom tasks disabled for on-device models.** Gemma is not smart enough to route free-form tasks to the right skill. Switch to a cloud LLM in Settings to unlock the text input.
- **Tasks stay in-app.** Starting a task no longer jumps to the home screen. You see progress in PokeClaw, then it goes to background when ready.

### v0.2.0 (2026-04-06)
- **Auto-reply now reads conversation context.** Before replying, the AI opens the chatroom and reads all visible messages on screen. It no longer forgets what was said 3 messages ago.
- **In-app update checker.** The app checks GitHub Releases once per day and prompts you to download if a newer version exists. No more manually checking.

### v0.1.0 (2026-04-06)
- Initial release. On-device Gemma 4 E2B with tool calling, accessibility-based phone control, auto-reply, task mode.

</details>

## Acknowledgments

PokeClaw exists because of [Gemma 4](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/) by [Google DeepMind](https://github.com/google-deepmind). Thank you to [Clément Farabet](https://github.com/clementfarabet), [Olivier Lacombe](https://github.com/olivierlacombe), and the entire Gemma team for shipping an open model with native tool calling under Apache 2.0. You made it possible for a solo developer to build a working phone agent in two nights. The [LiteRT-LM](https://ai.google.dev/edge/litert/llm/overview) runtime is what makes on-device inference practical.

Also inspired by the [OpenClaw](https://github.com/openclaw/openclaw) community 🦞 for proving that AI agents that actually do things are what people want.

And thank you to [Claude Code](https://claude.ai/code) by Anthropic. I'm a CS dropout with zero Android development experience. Claude Code made it possible for me to go from nothing to a working app in two nights. The future is wild.

## Trademark

PokeClaw is a trademark of Nicole / agents.io. The name "PokeClaw" and the PokeClaw logo may not be used to endorse or promote products derived from this software without prior written permission. Forks must be renamed before distribution.

## License

Apache 2.0

Contributors sign our [CLA](CLA.md) before their first PR is merged.

# Social Media

<h2 align="center">

[![shopee](https://img.shields.io/badge/shopee-200%2B-yellow.svg?style=flat)](https://shopee.co.id/infinixnote40bjm)

[![Youtube shopee_banjarmasin](https://img.shields.io/badge/YouTube-200%2B-yellow.svg?style=flat)](https://www.youtube.com/@shopee_banjarmasin)

[![Instagram shopee_banjarmasn](https://img.shields.io/badge/Instagram-2K%2B-yellow.svg?style=flat)](https://www.instagram.com/shopee_banjarmasin)

[![Twitter KipyMacho](https://img.shields.io/badge/Twitter-350%2B-yellow.svg?style=flat)](https://www.twitter.com/shopeebjm)
  
[![Tiktok Shopeebjm](https://img.shields.io/badge/TikTok-80%2B-yellow.svg?style=flat)](https://www.tiktok.com/@shopee.bjm)

[![Facebook shopee.bjm](https://img.shields.io/badge/Facebook-199%2B-yellow.svg?style=flat)](https://www.facebook.com/shopee.bjm)

[![Telegram](https://img.shields.io/badge/Telegram-77%2B-yellow.svg?style=flat)](http://t.me/shopeebjm)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-80%2B-yellow.svg?style=flat)](http://www.linkedin.com/in/kiplymacho)

</p>
<div height='45' align="center">
<h2>Contact me: <br>
<a href="https://github.com/shopeebjm"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/github.svg" height='50'> </a>
<a href="https://facebook.com/shopee.bjm"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/facebook.svg" height='50'> </a>
  
<a href="https://paypal.me/kiplymacho"> <img src="https://cdn.trakteer.id/images/embed/trbtn-red-6.png" height='50'> </a>
</h2>
</div>

# Follow Me :
‎
‎[![Messenger](https://img.shields.io/badge/Messengers-blue?style=for-the-badge&logo=messenger)](https://fb.me/shopee.bjm)
‎<a href="https://tiktok.com/@shopee.bjm"><img title="TikTok" src="https://img.shields.io/badge/-black?style=for-the-badge&logo=Tiktok"></a>
‎<a href="https://linktr.ee/kiplymacho" target="_blank"><img src="https://img.shields.io/badge/Socials-grey?style=for-the-badge&logo=linktree"></a>
‎<a href="https://github.com/shopeebjm" target="_blank"><img src="https://img.shields.io/badge/Github-blue?style=for-the-badge&logo=github"></a>
‎</p>
‎
‎[![Instagram](https://img.shields.io/badge/Instagram-Follow-red?style=for-the-badge&logo=instagram)](https://instagram.com/shopee_banjarmasin)
‎[![Blog](https://img.shields.io/badge/Website-Visit-yellow?style=for-the-badge&logo=blogger)](https://kiplymacho.blogspot.com)
‎[![Facebook](https://img.shields.io/badge/Facebook-Like-red?style=for-the-badge&logo=facebook)](https://facebook.com/shopee.bjm)
‎[![HalamanFacebook](https://img.shields.io/badge/Halaman-Facebook-sky?style=for-the-badge&logo=facebook)](https://facebook.com/httpcustomkiplymacho)
‎[![WhatsApp](https://img.shields.io/badge/WhatsApp-red?style=for-the-badge&logo=whatsapp)](https://wa.me/6285751032225)
‎[![Telegram](https://img.shields.io/badge/Forum-Diskusi-blue?style=for-the-badge&logo=forum)](https://t.me/shopeebjm)
‎<a href="https://youtube.com/@shopee_banjarmasin"><img title="YouTube" src="https://img.shields.io/badge/YouTube-@Shopee_Banjarmasin-red?style=for-the-badge&logo=Youtube"></a>
