---
name: crypto-scalping-trader
description: >
  Trading crypto otomatis dengan metode scalping di semua chain via Bankr.
  Gunakan skill ini ketika user ingin scalping, trading cepat, cari koin
  untuk scalping, analisis entry/exit scalping, atau trading otomatis jangka
  pendek. Trigger pada kata kunci seperti "scalping", "scalp", "trading cepat",
  "profit cepat", "entry scalping", "koin scalping", "auto trading", "trading otomatis".
metadata:
  version: "1.0.0"
  author: "herviana"
  emoji: "⚡"
---

# Crypto Scalping Trader ⚡

Skill trading otomatis dengan metode **scalping** di semua chain via Bankr.
Scalping adalah strategi trading jangka sangat pendek (menit hingga jam)
dengan target profit kecil tapi konsisten (1-5% per trade).

---

## Apa itu Scalping?

Scalping adalah strategi trading yang:
- ⏱️ Durasi trade: **1 menit - 4 jam**
- 🎯 Target profit per trade: **1-5%**
- 🔄 Frekuensi: **5-20 trade per hari**
- 🛡️ Stop loss ketat: **-1% hingga -3%**
- 📊 Mengandalkan **volume tinggi dan volatilitas**

---

## Cara Pakai

```
"Cari koin yang bagus untuk scalping hari ini"
"Analisis entry scalping untuk ETH"
"Set scalping otomatis untuk $50 per trade"
"Koin apa yang volatile sekarang?"
"Buat strategi scalping untuk modal $100"
"Cek sinyal scalping sekarang"
"Exit semua posisi scalping saya"
"Berapa profit scalping saya hari ini?"
```

---

## Kriteria Pemilihan Koin untuk Scalping

Agent akan memilih koin berdasarkan kriteria berikut:

### ✅ Koin BAGUS untuk Scalping:
- **Volume 24h** minimal $10 juta (likuiditas tinggi)
- **Volatilitas** 3-10% per hari (cukup gerak tapi tidak liar)
- **Spread bid-ask** rendah (< 0.5%)
- **Market cap** medium ($100M - $10B)
- **Trend** sedang dalam momentum naik atau konsolidasi
- **On-chain activity** tinggi (transaksi aktif)

### ❌ Koin yang DIHINDARI:
- Volume < $1 juta (susah exit)
- Baru launch < 7 hari (sangat berisiko)
- Spread terlalu lebar (> 1%)
- Sedang downtrend kuat
- Market cap < $10 juta (rentan manipulasi)

### 🏆 Koin Terbaik untuk Scalping (per chain):
```
Base Chain  : ETH, USDC pairs, token DeFi aktif di Base
Ethereum    : ETH, WBTC, UNI, LINK, AAVE
Solana      : SOL, JUP, BONK (hati-hati), RAY
BNB Chain   : BNB, CAKE, token BSC aktif
```

---

## Strategi Scalping Otomatis

### Strategi 1 — Momentum Scalping (Direkomendasikan)
```
Entry  : Saat harga breakout volume tinggi
Target : +2% dari entry
Stop   : -1% dari entry
Risk/Reward: 1:2
```

### Strategi 2 — Range Scalping
```
Entry  : Di support bawah range
Target : +3% (resistance atas range)
Stop   : -1.5% (di bawah support)
Risk/Reward: 1:2
```

### Strategi 3 — Trend Following Scalp
```
Entry  : Pullback di uptrend (setelah koreksi kecil)
Target : +3-5%
Stop   : -2%
Risk/Reward: 1:2.5
```

---

## Indikator yang Digunakan

Agent menganalisis indikator berikut sebelum entry:

| Indikator | Fungsi | Signal |
|-----------|--------|--------|
| RSI (14) | Overbought/Oversold | Entry saat RSI 40-60 |
| Volume | Konfirmasi momentum | Volume > rata-rata 20 periode |
| EMA 9/21 | Trend jangka pendek | EMA 9 di atas EMA 21 = bullish |
| Bollinger Bands | Volatilitas | Entry saat squeeze + breakout |
| MACD | Momentum | MACD line cross signal line |

---

## Manajemen Risiko Scalping

### Aturan Wajib:
- **Max per trade**: 10% dari total portfolio
- **Max loss per hari**: -5% total portfolio (auto stop trading)
- **Stop loss**: WAJIB dipasang sebelum entry
- **Jangan averaging down** saat scalping
- **Max posisi terbuka**: 3 posisi bersamaan

### Contoh Kalkulasi:
```
Modal total    : $500
Max per trade  : $50 (10%)
Target profit  : +$1 - $2.50 per trade (2-5%)
Max loss       : -$0.50 - $1.50 per trade (1-3%)
Target harian  : $10-25 (2-5% dari modal)
Max loss harian: -$25 (5% dari modal = stop trading)
```

---

## Perintah Trading Otomatis

```
# Set scalping otomatis
"Auto scalping ETH dengan modal $50, target 2%, stop loss 1%"

# Cari peluang scalping
"Scan semua chain untuk peluang scalping sekarang"

# Monitor posisi
"Cek semua posisi scalping saya yang terbuka"

# Exit manual
"Close semua posisi scalping saya sekarang"

# Laporan harian
"Tampilkan hasil scalping saya hari ini"
```

---

## Format Output Analisis

```
⚡ ANALISIS SCALPING — [TOKEN]

Chain    : Base / ETH / SOL
Harga    : $X.XX
Volume 24h: $XXM
Volatilitas: X%
RSI      : XX (Normal/Overbought/Oversold)
Trend    : Bullish / Bearish / Sideways

📊 REKOMENDASI:
Aksi     : BUY / SKIP / WAIT
Entry    : $X.XX
Target   : $X.XX (+X%)
Stop Loss: $X.XX (-X%)
Risk/Reward: 1:2

⚠️ Risk Level: LOW / MEDIUM / HIGH
```

---

## Format Output Laporan Harian

```
📊 LAPORAN SCALPING — [TANGGAL]

Total Trade  : XX
Profit Trade : XX (XX%)
Loss Trade   : XX (XX%)
Win Rate     : XX%

Profit Hari Ini : +$XX (+X%)
Loss Hari Ini   : -$XX (-X%)
NET PROFIT      : +$XX (+X%)

Trade Terbaik   : [TOKEN] +X%
Trade Terburuk  : [TOKEN] -X%

Status: ✅ PROFITABLE / ❌ LOSS
```

---

## Peringatan Penting

⚠️ **Scalping adalah strategi berisiko tinggi:**
- Membutuhkan eksekusi cepat dan disiplin ketat
- Biaya transaksi (gas fee) bisa makan profit jika terlalu sering
- Tidak cocok untuk pemula tanpa manajemen risiko
- Selalu gunakan stop loss — TIDAK ADA PENGECUALIAN
- Mulai dengan modal kecil dulu untuk belajar pola

---

## Integrasi dengan Skill Lain

Gunakan bersama skill berikut untuk hasil terbaik:

- **x-trending-crypto** → temukan koin yang mulai ramai
- **token-scam-analysis** → validasi keamanan token
- **Bankr core** → eksekusi trade langsung

---

## Referensi Tambahan

Lihat file berikut di folder `references/`:
- `indikator-scalping.md` — panduan lengkap membaca indikator
- `manajemen-risiko.md` — aturan ketat manajemen modal scalping
