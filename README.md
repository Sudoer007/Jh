# EPUB Stüdyo

Kotlin + Jetpack Compose (Material 3) ile yazılmış Android uygulaması.
- EPUB aç → bul/değiştir (Word'deki Ctrl+H gibi, tüm bölümlerde) → EPUB olarak kaydet
- EPUB → PDF (A4, görseller ve stillerle)

## APK üretme
**A) Android Studio:** klasörü aç → Gradle sync → Build > Build APK(s)
   (release APK: Build > Generate Signed App Bundle / APK ya da terminalde `gradle assembleRelease`;
   app/build/outputs/apk/release/ altında çıkar, debug anahtarıyla imzalıdır, doğrudan yüklenebilir)

**B) Bilgisayarsız (GitHub):** klasörü yeni bir GitHub deposuna yükle → Actions → "APK Derle" → Run workflow
   → bitince "EpubStudio-apk" artifact'ını indir.

Not: Kelime, etiketlerle bölünmüşse (ör. Mer<i>ha</i>ba) eşleşmez; düz metin içindeki kelimeler değişir.
