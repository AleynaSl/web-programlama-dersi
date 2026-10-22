# 🚀 Web Programlama I — Sistem Mimarları Operasyon Merkezi

**SCÜ Şarkışla UBYO | Bilişim Sistemleri ve Teknolojileri Bölümü**

Bu depo, Web Programlama I dersinin resmi **"Çevik (Agile) Operasyon Merkezi"**dir. Dönem boyunca tüm çeviriler, sunumlar, uygulama kodları ve soru-cevap dokümanları bu depo üzerinden, açık kaynak (open-source) sektör standartlarına uygun olarak yönetilecektir.

📌 **Kısa Özet:** Fork'la → Kendi kopyanda çalış → PR aç → Denetimden geç → Merge. Detaylar aşağıda.

---

## 📂 Depo Yapısı (Resmi Dokümantasyon Uyumlu)

Depo, ders yönergesindeki 5 ana kategori ve 14 modüle (MDN Learn, Vue.js, Three.js) birebir karşılık gelen klasörlerden oluşur. Her modül klasörünün içinde 4 standart içerik türü bulunur:

```
web-programlama1/
│
├── README.md                        ← bu dosya
│
├── 01-getting-started-1/            ← Getting Started (Takım 1)
│   ├── ceviri/
│   │   └── 2026-guz-kodbucuk.md
│   ├── sunum/
│   │   └── 2026-guz-kodbucuk.pdf
│   ├── uygulama/
│   │   └── v1-2026-kodbucuk/
│   │       ├── main.js
│   │       └── README.md
│   └── soru-cevap/
│       └── 2026-guz-kodbucuk.md
│
├── 02-getting-started-2/            ← Getting Started (Takım 2)
│   └── (aynı alt klasör yapısı: ceviri, sunum, uygulama, soru-cevap)
│
├── 03-core-modules-1/               ← Core Modules (Takım 3)
├── 04-core-modules-2/               ← Core Modules (Takım 4)
├── 05-core-modules-3/               ← Core Modules (Takım 5)
│
├── 06-extension-modules-1/          ← Extension Modules (Takım 6)
├── 07-extension-modules-2/          ← Extension Modules (Takım 7)
├── 08-extension-modules-3/          ← Extension Modules (Takım 8)
│
├── 09-vuejs-1/                      ← Vue.js Modules (Takım 9)
├── 10-vuejs-2/                      ← Vue.js Modules (Takım 10)
├── 11-vuejs-3/                      ← Vue.js Modules (Takım 11)
│
├── 12-threejs-1/                    ← Three.js Modules (Takım 12)
├── 13-threejs-2/                    ← Three.js Modules (Takım 13)
└── 14-threejs-3/                    ← Three.js Modules (Takım 14)
```

### 3 Katmanlı Mimari:

| Katman | Ne? | Örnek |
|---|---|---|
| 1. Modül | Resmi dokümantasyon modülü (1-14 arası) | `03-core-modules-1/` |
| 2. İçerik Türü | Çeviri / Sunum / Uygulama / Soru-Cevap | `ceviri/` |
| 3. Versiyon | Yıl + Dönem + Takım Adı | `2026-guz-kodbucuk.md` |

---

## 📝 Dosya İsimlendirme Kuralları

**Çeviri, Sunum, Soru-Cevap için:**

```
YIL-DONEM-TAKIMADI.uzanti
```

Örnekler:
- `2026-guz-kodbucuk.md`
- `2026-guz-yenitakim.pdf`
- `2027-guz-alfakubernetes.md`

**Uygulama için:**

```
vVERSIYON-YIL-TAKIMADI/
```

Örnekler:
- `v1-2026-kodbucuk/`
- `v2-2027-yenitakim/`

⚠️ **Neden yıl + takım adı?** Çünkü aynı modül her yıl farklı takımlar tarafından işlenir. Yıl ve takım adı olmadan dosyalar çakışır.

---

## 🔄 İş Akışı: Görevler Sisteme Nasıl Yüklenir?

Sektördeki gerçek yazılım ekipleri nasıl çalışıyorsa, biz de öyle çalışacağız. Bu depoya doğrudan dosya yükleme (Push) yetkiniz yoktur. Görevlerinizi **"Fork & Pull Request"** akışıyla teslim edersiniz.

### Adım 1: Projeyi Kopyalayın (Fork)

1. Bu sayfanın sağ üst köşesindeki **Fork** butonuna tıklayın.
2. **"Create Fork"** diyerek bu deponun kopyasını kendi GitHub profilinizde oluşturun.

### Adım 2: Kendi Kopyanızda Çalışın

1. Kendi profilinizdeki kopyaya gidin.
2. Bilgisayarınıza indirin (`git clone`) veya doğrudan GitHub arayüzünden dosya ekleyin.
3. Doğru modül klasörüne gidin ve dosyanızı ekleyin.

#### 📁 Nereye Koyacağım? (Karar Ağacı)

```
Issues panosunda hangi modülü seçtim?
→ Örn: Core Modules 1. Takım ise → 03-core-modules-1/
→ Örn: Vue.js 2. Takım ise       → 10-vuejs-2/

Hangi tür dosya hazırlıyorum?
→ Çeviri ise:     ceviri/
→ Sunum ise:      sunum/
→ Uygulama ise:   uygulama/
→ Soru-cevap ise: soru-cevap/

Dosya ismim ne olacak?
→ YIL-DONEM-TAKIMADI.md (örn: 2026-guz-kodbucuk.md)
```

### Adım 3: Katkı Talebi (Pull Request) Gönderin

1. Kendi fork'unuzda işinizi bitirin (Commit & Push).
2. Kendi deponuzun ana sayfasına gelin.
3. **"Contribute"** → **"Open Pull Request"** seçin.
4. Hedef: `mesutpolatgil/web-programlama1` → `main` dalı
5. **PR Başlığı:** `Modül XX - [Takım Adı] Teslimi`
   - Örnek: `Modül 03 - KodBucuk Teslimi`
6. **Açıklama:** Kısaca hangi alt konuları işlediğinizi ve ne yaptığınızı yazın (3-5 satır).

### Adım 4: Denetim (Code Review)

1. PR açtığınızda QA Asistanımıza bildirim gider.
2. QA Asistanı 48 saat içinde PR'ınızı inceler.
3. Eksik veya hatalı yerler varsa PR üzerinden yorum yapılır.
4. Gerekli düzeltmeleri yaptıktan sonra kendi deponuza tekrar push edin (PR otomatik güncellenir).
5. Hoca veya QA Asistanı nihai onayı verir ve PR merge edilir.

⚠️ **3 tur düzeltmeden sonra hâlâ eksikse PR reddedilir ve takım o hafta teslimattan 0 alır.**

---

## 💬 Commit Mesajı Formatı

```
modul-XX: [TakımAdı] kısa açıklama
```

**Örnekler:**

```
modul-03: KodBucuk ceviri eklendi
modul-03: KodBucuk slayt guncellendi
modul-03: KodBucuk uygulama kodlari eklendi
```

❌ **Kabul edilmeyen:** `asdf`, `update`, `değişiklik`, `final`, `son hali`

---

## ✅ PR Öncesi Kontrol Listesi

PR açmadan önce şunları kontrol edin:

- [ ] Issues'da seçtiğim doğru modül klasöründe miyim? (`03-core-modules-1/` gibi)
- [ ] Doğru içerik türünde miyim? (`ceviri/`, `sunum/`, `uygulama/`, `soru-cevap/`)
- [ ] Dosya ismi doğru formatta mı? (`2026-guz-takimadi.md`)
- [ ] Uygulama klasöründe kodları açıklayan bir `README.md` var mı?
- [ ] Çeviri dosyasının en başında yasal uyarı var mı?
- [ ] Commit mesajı standart formatta mı?
- [ ] PR başlığı formatı doğru mu?
- [ ] Başka takımın klasörüne veya dosyasına dokunmadım, değil mi?

---

## 📎 Örnek Teslim

**Senaryo:** 3. Modül (`03-core-modules-1`), "KodBucuk" takımı.

**Ekleyeceği dosyalar:**

```
03-core-modules-1/
├── ceviri/
│   └── 2026-guz-kodbucuk.md
├── sunum/
│   └── 2026-guz-kodbucuk.pdf
├── uygulama/
│   └── v1-2026-kodbucuk/
│       ├── main.js
│       └── README.md
└── soru-cevap/
    └── 2026-guz-kodbucuk.md
```

**Commit mesajları:**

```
modul-03: KodBucuk ceviri eklendi
modul-03: KodBucuk slayt eklendi
modul-03: KodBucuk uygulama kodlari eklendi
```

**PR başlığı:**

```
Modül 03 - KodBucuk Teslimi
```

---

## 📅 Teslim Kuralları

| Kural | Detay |
|---|---|
| **Deadline** | Sunumdan önceki Cuma 23:59 |
| **Geç Teslim** | 24 saat içinde %20 kırılır, sonrası kabul edilmez |
| **PR Hedefi** | `main` dalı |
| **PR Başlığı** | `Modül XX - [Takım Adı] Teslimi` |
| **Commit Formatı** | `modul-XX: TakimAdi ne-yaptim` |

---

## 📜 Yasal Uyarı ve Telif

Bu depo altındaki içerikler eğitim amacıyla hazırlanmaktadır.

Öğrenci takımları tarafından hazırlanan **tüm çeviri dosyalarının en üstünde** şu ibare yer almak zorundadır:

> **Uyarı:** Bu içerik, SCÜ Şarkışla UBYO Web Programlama I dersi kapsamında tamamen eğitim amaçlı çevrilmiş ve derlenmiştir. Orijinal dokümantasyon kaynakları (MDN Web Docs, Vue.js, Three.js vb.) kendi orijinal lisanslarına (CC-BY-SA, MIT) tabidir. Bu çalışmanın hiçbir ticari amacı yoktur.

**Yasal uyarı olmayan çeviri PR'ları reddedilir.**

---

## 🎯 İlk Göreviniz

1. Takım kurun (3-4 kişi, sınıf temsilcisi koordine eder).
2. Modül seçin (14 modülden biri).
3. GitHub Issues sekmesinde, sınıf temsilcisinin açtığı **"Dönem İçi Konu Dağılım Listesi"** başlığı altına yorum olarak yazın.
4. Sunumunuzdan önceki Cuma 23:59'a kadar ilgili modül klasörüne ilk PR'ınızı açın.

---

## 📞 İletişim

- **Teknik sorular:** GitHub Discussions (WhatsApp değil!)
- **Acil durumlar:** [Hoca/Asistan e-posta]
- **PR incelemesi:** QA Asistanı + Hoca

---

**Tüm takımlara mühendislik simülasyonunda başarılar dilerim.**  
**Kodunuz bug'sız, render'ınız pürüzsüz olsun!**
