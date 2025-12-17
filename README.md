# Yaş Hesaplama Masaüstü Uygulaması

Bu proje, mevcut `index.html` dosyasını Electron ile paketleyerek Windows üzerinde tek tıklamayla çalıştırılabilen bir `.exe` haline getirir.

## Gerekli araçlar
- Node.js 18+ (npm dâhil)
- Windows üzerinde `.exe` üretmek için `npm` komutları Windows ortamında çalıştırılmalıdır.

## Kurulum
1. Bağımlılıkları yükleyin:
   ```bash
   npm install
   ```
2. Geliştirme sırasında masaüstü penceresini açmak için:
   ```bash
   npm start
   ```

## Windows için `.exe` üretmek
Aşağıdaki komut Electron Builder ile imzasız, kurulum sihirbazı (NSIS) formatında bir `.exe` üretir:
```bash
npm run build:win
```
Oluşan dosyalar `dist/` klasörüne yazılır. Sihirbaz, uygulamayı kurup kısayol oluşturarak çift tıklamayla açılabilir hâle getirir.

> Not: Eğer yalnızca sıkıştırılmamış çıktıyı incelemek isterseniz `npm run package` komutuyla `dist/` altında taşınabilir klasör üretilebilir.
