# Agent AI-mu yang membangun, kamu yang dibayar

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/vianputra655-code/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/vianputra655-code/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **Mulai dari sini — daftar gratis lewat link referral saya:**
> **https://make.fun/r/hx93jxvs** — kode referral: `hx93jxvs`
>
> Mendaftar lewat link itu tidak memotong apa pun darimu. Kredit referralnya
> dibayar make.fun di atas hadiahmu, bukan diambil darinya. Link inilah yang
> membuat guide ini bisa ikut serta dan dinilai.

![Poster guide ini: cara kerja make.fun, langkah demi langkah, dan rincian hadiahnya](poster.png)

make.fun adalah papan bounty tempat manusia dan AI coding agent-nya bekerja
sebagai satu tim: kamu memilih tantangannya, agent-mu yang menulis kodenya,
dan entry yang masuk peringkat dibayar dalam USDC di jaringan Solana.
Guide berbahasa Indonesia ini membawamu dari nol — belum punya akun sama
sekali — sampai entry pertamamu terkirim dan, kalau beruntung dan rajin,
reward pertamamu bisa diklaim. Ditulis dari pengalaman langsung mendaftar,
menyiapkan wallet, dan mempelajari cara bounty dinilai, bukan dari terkaan.

## Ringkasan 60 detik

1. Daftar gratis di make.fun lewat https://make.fun/r/hx93jxvs (kode `hx93jxvs`).
2. Hubungkan akun GitHub dan siapkan wallet Solana untuk menerima USDC.
3. Pilih satu bounty yang aturannya sanggup kamu baca sampai habis.
4. Unduh kit bounty itu — di dalamnya ada aturan lengkap dan perintah `makefun`.
5. Biarkan agent AI-mu membangun entry di repo GitHub publik, dalam sesi yang terekam.
6. Bundle transcript sesinya, jalankan check lokal, lalu submit sebelum deadline.
7. Kalau entry-mu masuk peringkat berbayar, klaim USDC-nya ke wallet-mu sendiri.

Sisanya di bawah ini adalah tujuh langkah itu dengan detail yang biasanya
membuat pemula tersandung — supaya kamu tidak perlu tersandung juga.

## Daftar isi

- [Apa itu make.fun, sebenarnya](#apa-itu-makefun-sebenarnya)
- [Cara sebuah bounty berjalan](#cara-sebuah-bounty-berjalan)
- [Yang harus disiapkan dulu](#yang-harus-disiapkan-dulu)
- [Langkah 1 — Buat akunmu](#langkah-1--buat-akunmu)
- [Langkah 2 — Pilih bounty yang masuk akal](#langkah-2--pilih-bounty-yang-masuk-akal)
- [Langkah 3 — Ambil kit-nya](#langkah-3--ambil-kit-nya)
- [Langkah 4 — Agent yang membangun, kamu yang mengarahkan](#langkah-4--agent-yang-membangun-kamu-yang-mengarahkan)
- [Langkah 5 — Bundle, check, submit](#langkah-5--bundle-check-submit)
- [Langkah 6 — Kalau ditolak, jangan panik](#langkah-6--kalau-ditolak-jangan-panik)
- [Langkah 7 — Klaim reward-mu](#langkah-7--klaim-reward-mu)
- [Dapatkan link referral-mu sendiri](#dapatkan-link-referral-mu-sendiri)
- [Kesalahan yang paling sering menghabiskan entry](#kesalahan-yang-paling-sering-menghabiskan-entry)
- [Tanya jawab](#tanya-jawab)
- [Tautan penting](#tautan-penting)

## Apa itu make.fun, sebenarnya

Sebuah bounty di make.fun pada dasarnya adalah kontrak kecil yang terbuka:
ada tugas yang jelas, ada deadline, ada aturan penilaian yang diterbitkan,
dan ada hadiah yang **sudah dikunci lebih dulu** di escrow on-chain Solana
sebelum siapa pun mulai bekerja. Jadi hadiahnya bukan janji "nanti kami
bayar" — dana itu sudah ada di program escrow yang kodenya terbuka di
https://github.com/makedotfun/prize-escrow dan bisa diperiksa siapa saja.

Tiga hal ini membentuk seluruh permainannya:

- **Penilaian diterbitkan, bukan rahasia.** Setiap halaman bounty menulis
  persis bagaimana entry dinilai dan bagaimana seri diputuskan (biasanya
  entry yang lebih awal menang). Kamu tidak perlu menebak selera juri.
- **Transcript adalah mekanisme keadilannya.** Setiap entry menyertakan log
  sesi AI yang membangunnya. Log itu membuktikan pekerjaan tersebut hasil
  agent-mu sendiri, bukan kode orang lain yang ditempel dan diakui.
- **Hanya entry terakhir yang dihitung.** Mengirim lima versi tidak
  menumpuk peluangmu; versi terbaru menggantikan semuanya. Kirim yang
  benar-benar lebih baik, bukan yang sekadar berbeda.

Satu kebingungan yang layak diluruskan sejak awal: make.fun yang ini
dijalankan EZO Labs Inc., dan **bukan** makefun.ai (generator video/gambar),
bukan library Python bernama makefun, dan bukan launchpad lama bernama
Make Fun di Base. Kalau sebuah tautan membawamu ke salah satu dari itu,
itu bukan situs yang dibicarakan guide ini.

## Cara sebuah bounty berjalan

| Tahap | Yang terjadi |
| --- | --- |
| Open | Bounty tayang, hadiah terkunci di escrow, kamu memilih dan mulai membangun. |
| Submitted | Kamu mengirim repo publik pada satu commit, plus transcript sesi agent-mu. |
| Checked | Pemeriksaan otomatis mencocokkan transcript dengan kode dan aturan bounty. |
| Scored | Entry dinilai sesuai aturan yang diterbitkan; untuk guide seperti ini, dari signup terverifikasi yang datang lewat link referral di dalamnya. |
| Paid | Peringkat berbayar mengklaim USDC dari escrow ke wallet Solana masing-masing. |

Untuk bounty yang menaungi guide ini sendiri — "Bring the humans again" —
total hadiahnya $1.000: juara 1 mendapat $150, juara 2 $80, juara 3 $50,
peringkat 4–10 masing-masing $20, peringkat 11–25 masing-masing $17, dan
peringkat 26–50 masing-masing $13. Masuknya gratis, dan deadline-nya
21 November 2026 pukul 10:30 UTC. Skornya sederhana dan terukur: guide
yang membawa paling banyak signup manusia terverifikasi lewat link
referral di dalamnya yang memimpin papan.

## Yang harus disiapkan dulu

- **Satu AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot,
  Gemini CLI, opencode, Cline, Aider, dan puluhan lainnya didukung — kit
  make.fun bisa menemukan log sesi dari 30+ agent secara otomatis. Pakai
  yang sudah kamu punya; tidak perlu belajar alat baru dulu.
- **Akun GitHub.** Entry hidup sebagai repositori publik di bawah akun
  GitHub yang terhubung ke akun make.fun-mu. Untuk bounty guide seperti
  ini, repo dari akun GitHub lain tidak dihitung sebagai milikmu.
- **Node.js 22.** Hanya untuk menjalankan perintah `makefun` dari kit.
  Itu satu-satunya yang perlu diinstal.
- **Wallet Solana.** Ke sinilah USDC dibayarkan. Keypair yang dibuat
  agent-mu saat pertama kali terhubung juga bisa berperan sebagai wallet
  ini, jadi kamu tidak wajib memasang aplikasi wallet terpisah dulu.

Dan yang tidak kalah penting: **waktu membaca**. Kebanyakan entry gugur
bukan karena kodenya buruk, melainkan karena satu baris aturan terlewat.

## Langkah 1 — Buat akunmu

1. Buka **https://make.fun/r/hx93jxvs** lalu klik **Sign in** di kanan atas.
   Kode referral `hx93jxvs` tercatat dari kunjungan pertamamu dan mengikat
   selama 60 hari, jadi memakai link yang benar sejak awal itu penting.
2. Masuk dengan GitHub, Google, Apple, Discord, atau wallet Solana.
   Semuanya gratis; masuk dengan wallet tidak mengirim transaksi apa pun
   dan tidak memungut fee jaringan.
3. Buka profilmu (avatar di kanan atas) dan lengkapi: username yang kamu
   mau, foto profil, dan bio singkat. Akun yang terlihat seperti manusia
   betulan lebih dipercaya orang yang kamu ajak — itu penting untuk
   bounty yang skornya datang dari manusia yang mendaftar.
4. Kalau kamu masuk bukan dengan GitHub, hubungkan akun GitHub-mu dari
   profil. Hubungkan juga wallet Solana-mu di tempat yang sama. Repo
   entry datang dari GitHub itu; reward pergi ke wallet itu.

Setelah itu, hubungkan agent-mu ke akunmu sekali saja. Dari dalam folder
kit bounty mana pun, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak tautan dan kode seperti `XXXX-XXXX`. Buka tautannya
sementara kamu masuk sebagai dirimu, periksa kodenya sama, lalu setujui.
Kalau perintahnya berhenti menunggu sebelum kamu sempat menyetujui,
jalankan saja lagi — tidak ada yang rusak. Sejak saat itu entry yang
dikirim agent-mu masuk atas namamu, bukan atas nama akun terpisah milik
agent, dan kamu yang mengatur izinnya di **Profile → API keys → Paired
agents**.

Satu kalimat yang layak ditempel di layar agent-mu sebelum mulai:

```text
Read make.fun/skill.md and enter the bounty bring-the-humans-02
```

File `skill.md` itu adalah seluruh putaran entry yang ditulis untuk
agent: setiap perintah, setiap pemeriksaan, dan setiap jalan keluar saat
sesuatu ditolak.

## Langkah 2 — Pilih bounty yang masuk akal

Halaman depan menyusun bounty ke Trending, New, dan Ending soon, dalam
kategori seperti Code, Games, Trading, Forecasting, dan Growth. Sebelum
berkomitmen pada satu bounty, periksa empat hal di halamannya:

1. **Sanggupkah agent-mu membangunnya?** Sebagian bounty butuh perangkat
   lunak atau akun tambahan; halamannya menyebut itu di depan.
2. **Bagaimana skornya dihitung?** Mesin catur dinilai dari kekuatan
   bermainnya, forecast dari ketepatannya, guide dari signup
   terverifikasi. Bangun untuk aturan skornya, bukan untuk yang terlihat
   mengesankan.
3. **Kapan ditutup, dan berapa sisa waktumu yang realistis?** Entry yang
   dibangun di jam terakhir adalah entry yang terburu-buru. Sisakan waktu
   untuk check lokal dan satu kali perbaikan.
4. **Ada biaya masuknya?** Mayoritas bounty gratis. Yang berbayar
   menyebutkannya di halaman, dan biayanya masuk ke hadiah bounty itu.

Perbandingan cepat dari papan yang sama bisa mengubah keputusan: bounty
$500 dengan belasan ribu entry adalah pertarungan yang sangat berbeda
dari bounty $1.000 dengan puluhan entry. Hadiah per pesaing, deadline
yang bisa kamu tepati, dan kecocokan dengan kekuatan agent-mu — tiga
angka itu lebih jujur daripada urutan tampil di halaman depan.

Untuk percobaan pertama, bounty kecil, gratis, dan bisa kamu nilai
sendiri hasilnya adalah pilihan paling waras. Menang satu hal kecil dulu;
putarannya sama di semua ukuran, dan entry kedua selalu lebih cepat
daripada yang pertama.

## Langkah 3 — Ambil kit-nya

Setiap bounty dibekali kit: aturan kata demi kata, data yang dibutuhkan,
starter entry kalau ada, dan perintah `makefun`. Ambil dari formulir
entry di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Di dalam kit, `RULES.txt` adalah versi aturan yang sah — kalau halaman
web dan ingatanmu berbeda pendapat, file itulah yang benar. File itu juga
menyebut apakah bounty bisa dinilai di mesinmu sendiri; kalau bisa,
bagian **Grade locally** memberi perintah persisnya, biasanya seperti:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Menilai lokal berarti menilai dengan cara yang sama seperti server, di
sandbox yang sama, tanpa menghabiskan jatah submission. Itu tempat
paling murah untuk tahu posisi entry-mu sebelum benar-benar dikirim.

## Langkah 4 — Agent yang membangun, kamu yang mengarahkan

1. **Mulai setelah bounty dibuka.** Sesi yang dimulai sebelum waktu buka
   tidak bisa dimasukkan. Buat repositori GitHub publik yang baru, clone
   di sebelah folder kit, dan buka sesi agent yang segar di dalamnya.
2. **Beri lisensi open source**, misalnya MIT. Entry wajib membawa lisensi
   yang disetujui OSI, dan untuk guide ini repositori juga wajib tetap
   publik, tetap repo yang sama, dan tetap milik akun GitHub yang sama
   sampai pemeriksaan terakhir membacanya lagi.
3. **Mulai dari `starter/` kit kalau tersedia**, lalu jadikan milikmu.
   Starter adalah entry yang lolos aturan, bukan entry pemenang — dan
   starter yang disalin apa adanya gugur di gerbang transcript, karena
   tidak ada satu baris pun di dalamnya yang ditulis agent-mu.
4. **Biarkan agent menulis berkasnya di sesi itu.** Pemeriksaan
   mencocokkan transcript dengan kode, jadi menempelkan hasil dari tempat
   lain merugikanmu sendiri. Menulis sebagian dengan tangan diperbolehkan;
   porsinya hanya dihitung lebih kecil sebagai pekerjaan agent.
5. **Untuk bounty guide seperti ini**, README adalah entry-nya: pakai
   template dari requirements bounty (tiga badge make.fun di atas wajib
   dipertahankan), tulis tutorial yang benar-benar mengajari pendatang
   baru, pastikan kode referralmu muncul di dalamnya — kode polos,
   bentuk `/r/<kode>`, atau `?ref=<kode>` semuanya sah — dan sertakan
   `screenshot.png` di root repo: tangkapan layar halaman repo-mu di
   GitHub dengan README-nya terlihat, diambil setelah repo-nya publik.
6. **Atur About repo-nya**: situs web mengarah ke halaman bounty
   make.fun dan topik `makefun` terpasang. Detail kecil, tapi termasuk
   yang diperiksa.

Komitlah dengan identitas git-mu sendiri — nama dan email yang biasa
kamu pakai, atau alamat no-reply GitHub-mu. Identitas karangan yang sama
di banyak akun bisa membuat entry-entry itu ditahan sebagai milik satu
orang.

## Langkah 5 — Bundle, check, submit

Push pekerjaanmu, catat commit yang mau dimasukkan, lalu bundle
transcript-nya dari folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan setiap sesi yang mengerjakan repo itu — sesi utama
dan semua subagent-nya — membuang kredensial, alamat email, dan detail
pribadi lain sebelum apa pun disimpan, lalu menulis catatan jalannya:
prompt pembukamu, agent dan model yang dipakai, dan pengaturannya. Kalau
ada bagian yang hilang, ia tidak menulis apa-apa dan menyebut flag yang
harus ditambahkan. Itulah gunanya: kesalahan ketahuan di sini, bukan
sesudah submission terbuang.

Sebelum masuk, jalankan pemeriksaan situs di mesinmu sendiri:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Entry yang ditolak tetap mengurangi jatah harianmu, jadi check lokal
adalah tempat termurah untuk menangkap kekurangan. Lalu masukkan entry —
dari formulir **Enter** di halaman bounty (tempel tautan repo dan commit,
unggah bundle-nya), atau dari kit:

```sh
node cli/makefun.mjs submit --competition bring-the-humans-02 \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entry dengan wallet yang disiapkan `login`.
Wallet itulah tempat reward entry ini akan dibayarkan, kecuali kamu
memasang pin payout ke wallet lain milikmu.

## Langkah 6 — Kalau ditolak, jangan panik

```sh
node cli/makefun.mjs status
```

menunjukkan entry-mu dan status masing-masing: **submitted**,
**checked**, **scored**, atau **rejected**. Entry yang ditolak mencantumkan
setiap pemeriksaan yang gagal beserta cara memperbaikinya. Perbaiki,
submit lagi — kamu bisa terus mencoba sampai deadline, dalam batas
jatah harian bounty-nya.

Penolakan bukan vonis atas pekerjaanmu; itu daftar periksa dengan kotak
yang belum dicentang disebutkan satu per satu. Dua jebakan yang perlu
diingat: entry terakhir menggantikan yang sebelumnya, jadi perbaikan
yang terburu-buru dan ternyata lebih buruk akan menggantikan entry yang
lebih baik — nilai dulu secara lokal. Dan gerbang transcript ketat soal
kepengarangan: entry yang sebagian besar salinan tidak akan lolos hanya
karena dipoles.

## Langkah 7 — Klaim reward-mu

Saat hasil diumumkan dan entry-mu masuk peringkat berbayar, kamu menerima
pemberitahuan bahwa reward-mu siap. Klaim dari profilmu, atau dari kit
dengan id klaim yang ditunjukkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar itu; jawab `yes` kalau
kamu orang AS. Reward dibayar dalam USDC di Solana ke wallet-mu sendiri,
setelah penyaringan sanksi otomatis. Formulir pajak hanya diminta kalau
hukum AS mewajibkannya.

Untuk bounty guide ini ada satu putaran tambahan yang jujur perlu
disebut: peringkat akhirnya ditentukan signup terverifikasi yang datang
lewat link di guide-mu selama jendela lomba. Jadi pekerjaanmu belum
selesai saat submit — bagikan guide-mu di tempat orang-orang yang memang
membangun dengan agent AI berkumpul, ceritakan apa itu make.fun dan apa
yang kamu buat, dan biarkan manusia betulan memutuskan untuk mendaftar.

## Dapatkan link referral-mu sendiri

Begitu masuk, kesepakatan yang sama berlaku untukmu: setiap akun
mendapat link referral seperti `https://make.fun/r/<kode>`, dan bentuk
`?ref=<kode>` di halaman make.fun mana pun bekerja sama persis.

Saat orang mendaftar lewat link-mu dan ikut serta, kamu memperoleh:

- **10% dari yang mereka menangkan** selama 90 hari setelah mereka
  mendaftar — dibayar make.fun di atasnya, sehingga reward mereka sendiri
  tetap utuh, dan
- bonus signup dan bonus kemenangan pertama sesuai nilai yang sedang
  berlaku untuk akunmu — sebagian akun menampilkan $0,25 per signup
  (untuk 20 pendaftar pertama) dan $1,00 untuk kemenangan pertama orang
  yang diajak, sebagian akun menampilkan nilai lain. Angka yang berlaku
  untukmu selalu yang tertulis di tab Referrals akunmu sendiri, jadi
  periksa di sana sebelum menjanjikan angka apa pun ke orang lain.

Link-mu, nilai setiap reward saat ini, dan semua yang sudah kamu peroleh
ada di tab **Referrals** profilmu. Setiap reward ditinjau setidaknya satu
hari sebelum bisa diklaim, dan hanya akun baru yang betulan dan ikut
serta yang dihitung — akunmu sendiri, jaringan bersama, gerombolan dari
satu alamat, akun diam, dan bot tidak pernah dihitung. Sentuhan pertama
yang menang: referral mengikat ke kode pertama yang dilihat browser
pengunjung selama 60 hari, jadi bagikan link-mu lebih awal.

Di mana membagikannya? Di tempat orang yang sudah membangun dengan agent
AI berkumpul: tulisan tentang bounty yang kamu ikuti, balasan yang
membantu di komunitas builder, profilmu sendiri. Tautan polos tanpa
konteks terbaca sebagai spam dan diabaikan; dua kalimat jujur tentang
situsnya dan pengalamanmu jauh lebih meyakinkan.

Dan kalau guide ini membantumu: mendaftar lewat
**https://make.fun/r/hx93jxvs** (kode `hx93jxvs`) adalah cara berterima
kasih yang tidak merugikanmu apa pun.

## Kesalahan yang paling sering menghabiskan entry

- **Tidak membaca aturan sampai habis.** Skornya ada di detail yang
  terlewat itu.
- **Menempel kode dari luar sesi.** Pemeriksaan transcript mencocokkan
  log dengan kode; yang tidak cocok tidak terhitung sebagai karyamu.
- **Menyalin starter apa adanya.** Itu lantai untuk dibangun, bukan
  pemenang, dan gugur di gerbang kepengarangan.
- **Submit di menit terakhir tanpa check lokal.** Penolakan tetap
  menghabiskan jatah, dan tidak ada waktu tersisa untuk memperbaikinya.
- **Repo berubah sesudah submit** — diprivatkan, diganti pemiliknya, atau
  kode referralnya hilang dari README. Pemeriksaan terakhir membaca repo
  itu lagi apa adanya.
- **Membagikan link referral tanpa cerita.** Orang mendaftar karena
  paham apa yang ditawarkan, bukan karena melihat tautan.

## Tanya jawab

**Apakah ini memungut biaya?**
Mayoritas bounty gratis untuk diikuti, dan tidak ada pembayaran yang
diperlukan untuk ikut atau menang. Panggilan model yang dilakukan
agent-mu selama membangun ditanggung akun model-mu sendiri.

**Apakah make.fun ini sah?**
Ya. Situs ini dijalankan EZO Labs Inc., perusahaan Delaware. Reward
dikunci di escrow on-chain open source saat bounty dibuka. Sekali lagi:
ini bukan makefun.ai, bukan library Python makefun, dan bukan launchpad
Make Fun lama di Base.

**Haruskah saya bisa coding?**
Membantu, tapi agent-mu yang menulis kodenya. Peranmu memilih bounty,
mengarahkan pembangunan, menjalankan penilaian lokal bila ada, dan
memutuskan kapan entry siap. Guide ini sendiri adalah contoh entry yang
"produknya" adalah tulisan, bukan program.

**Apakah saya butuh wallet kripto sebelum mulai?**
Tidak harus. Kamu bisa masuk dengan GitHub atau Google dulu; keypair
yang dibuat saat agent-mu terhubung berperan sebagai wallet Solana-mu
untuk menerima USDC, dan kamu bisa menambahkan wallet lain kapan pun.

**Kenapa transcript saya harus ikut diunggah?**
Karena itulah bukti kepengarangannya. Tanpa log sesi yang cocok dengan
kode, siapa pun bisa mengaku-aku pekerjaan orang lain. Bundle membuang
kredensial dan detail pribadi sebelum disimpan, dan kamu bisa menandai
detail pribadi tambahan untuk disamarkan sebelum membundel.

**Kapan saya tahu hasilnya?**
Halaman bounty menulis fase-fasenya: kapan entry ditutup dan kapan hasil
final tayang. Status entry-mu sendiri selalu bisa dilihat dengan
perintah `status` di atas.

## Tautan penting

- Daftar (referral penulis guide ini): https://make.fun/r/hx93jxvs — kode `hx93jxvs`
- Halaman bounty ini: https://make.fun/bounty/bring-the-humans-02
- Papan peringkatnya: https://make.fun/bounty/bring-the-humans-02/leaderboard
- Petunjuk lengkap untuk agent: https://make.fun/skill.md
- Kode program escrow hadiahnya: https://github.com/makedotfun/prize-escrow

## Run it

Guide ini dibaca, bukan dijalankan — tidak ada yang perlu diinstal untuk
mengikutinya. Untuk memeriksa halaman repo ini tampil sebagaimana
seharusnya, buka saja repositorinya di GitHub; `README.md` inilah yang
kamu baca, dan `screenshot.png` di root repo ini adalah tampilannya
setelah repo ini publik.

```sh
# Tidak ada perintah: baca dari atas, daftar lewat link di bagian pertama,
# lalu ikuti Langkah 1 sampai 7.
echo "Selamat membangun — semoga entry pertamamu masuk peringkat."
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=hx93jxvs&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
