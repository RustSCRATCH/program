![RustSCRATCH Header](https://raw.githubusercontent.com/RustSCRATCH/ikonlar/main/RustSCRATCH.png)

![Release](https://img.shields.io/badge/Release-v0.1.0-blue.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Rust](https://img.shields.io/badge/Rust-x86__64--pc--windows--gnu-orange.svg)
![Tauri](https://img.shields.io/badge/Tauri-v2-FFC131.svg)

**RustSCRATCH**, PenguinMod tabanlı web yapısını Rust ve Tauri V2 gücüyle masaüstüne taşıyan, ultra hafif ve yüksek performanslı bir blok kodlama editörüdür.

---

## 🚀 Öne Çıkan Özellikler

* **PenguinMod Tabanlı Yapı:** Scrooch 3 araçlarıyla optimize edilmiş, yerel (local) dosyalar üzerinden doğrudan çalışan gelişmiş Scratch mimarisi.
* **Rust & Tauri V2 Mimarisi:** Ağır WebView veya Electron bağımlılıkları olmadan yüksek performans ve düşük bellek (RAM) kullanımı.
* **Küçük Dosya Boyutu:** MSVC yerine **GNU (`x86_64-pc-windows-gnu`)** araç zinciri kullanılarak minimum sistem gereksinimi ve küçük paket boyutu hedeflendi.
* **Açık Kaynak & Esnek:** Tamamen özgür geliştirme imkânı sunan MIT lisansı.

---

## 🛠️ Kullanılan Teknolojiler

* **Yazılım Dili:** Rust
* **Masaüstü Çerçevesi (Framework):** Tauri v2
* **Arayüz & Web Altyapısı:** HTML5 / JS (Scrooch 3 ile derlenmiş PenguinMod tabanlı yerel web varlıkları)
* **Derleyici Toolchain:** `stable-x86_64-pc-windows-gnu` (MSVC'ye kıyasla ~700 MB daha hafif geliştirme ortamı)

---

## 📥 İndirme ve Kaynak Kodlar

Projenin tüm kaynak kodlarını ve derlemeye hazır paketini doğrudan indirmek için aşağıdaki bağlantıyı kullanabilirsiniz:

👉 **[RustSCRATCH Kaynak Kodunu İndir (.zip)](https://raw.githubusercontent.com/RustSCRATCH/program/main/RustScratch.zip)**

---

## 📦 Sıfırdan Derleme (Build) Rehberi

Eğer uygulamayı kendiniz derleyip `.exe` dosyasını üretmek istiyorsanız aşağıdaki adımları sırasıyla takip edin:

### 1. Ön Gereksinimler
* Bilgisayarınızda **Rust** kurulu olmalıdır.
* Windows için **MSYS2 / UCRT64** (MinGW GCC) ortamının kurulu ve `PATH` değişkenine eklenmiş olması gerekir.

### 2. Kurulum ve Derleme Adımları

1. İndirdiğiniz `RustScratch.zip` dosyasını bir klasöre ayıklayın.
2. Komut Satırını (CMD veya PowerShell) klasörün içinde açın.
3. Derleyici araç zincirinin aktif olduğundan emin olun:
   ```cmd
   set PATH=C:\(KURULDUPU YER)\msys2\ucrt64\bin;%PATH%
   ```
4. Derlemeyi başlat
   ```cmd
   cargo tauri build
   ```   
