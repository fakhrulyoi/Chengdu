# Trip Chengdu · 7–13 Jan 2027

App trip (jadual, peta laluan, kos & bajet, cuti AL, senarai barang, apps), dwibahasa BM/EN. Boleh dipasang di telefon dan dibuka offline.

**Link app:** https://fakhrulyoi.github.io/Chengdu/ (lepas GitHub Pages diaktifkan)

## Aktifkan GitHub Pages (sekali sahaja)
Settings → Pages → Build and deployment → **Source: Deploy from a branch** → **Branch: `main` / `(root)`** → Save.
Tunggu 1–2 minit, kemudian buka link di atas.

## Sync: semua orang nampak perubahan
- Semua kandungan trip ada dalam **`data.json`** dalam repo ni.
- App setiap orang semak `data.json` terbaru bila app dibuka dan setiap 1 minit.
- **Admin edit terus dalam app:** buka tab **Apps → Admin: edit & sync**, masukkan token GitHub (sekali sahaja, disimpan dalam telefon kau sahaja). Lepas tu tekan **✎ Edit** di setiap tab. Bila tekan Simpan, app commit ke repo dan semua orang nampak dalam ~1 minit.
- Boleh juga edit `data.json` terus di GitHub (ikon pensel → Commit).

### Buat token admin
GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens → Generate new token**
- Repository access: **Only select repositories → Chengdu**
- Permissions → Repository permissions → **Contents: Read and write**
- Salin token (`github_pat_…`) dan tampal dalam app.

Untuk co-admin, buat token berasingan untuk dia, atau tambah dia sebagai collaborator di repo ni dan dia buat token sendiri. **Jangan kongsi token dalam group chat.**

## Makan halal
Tab **Makan** senaraikan tempat halal ikut kawasan (Chengdu, Siguniang, Bipenggou, Xiling, Dujiangyan, TFU), dengan pautan peta dan sumber. Setiap hari dalam Jadual pun tunjuk tempat halal untuk kawasan hari tu. Admin boleh tambah atau edit dalam app.

## Split bill
Tab **Duit → Split bill**:
- **Kira cepat:** bahagi satu bil sama rata (¥ atau RM). Tak disimpan.
- **Bil group:** admin rekod siapa bayar apa, dan untuk siapa. App kira baki setiap orang dan cara langsai yang paling sedikit pindahan duit, dan boleh hantar terus ke WhatsApp. Kadar ¥→RM boleh diedit.

## Perbelanjaan group
Tab **Kos** papar terus data dari Google Sheet *Expenses Tracker* (oleh CA Muhammad Aiman). Sheet mesti dikongsi sebagai **Anyone with the link → Viewer** supaya app boleh baca. Link sheet boleh ditukar dalam app (Kos → ✎ Edit bajet).

## Nota
- Senarai barang disimpan dalam telefon setiap orang. Guna butang **Kongsi ke WhatsApp** untuk tunjuk progress.
- Peta (`map.svg` / `map.png`) ialah imej tetap. Kalau tempat atau laluan berubah, peta perlu dijana semula.
