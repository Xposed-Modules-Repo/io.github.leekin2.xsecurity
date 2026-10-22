# XSecurity

**Region-gated Security app features, unlocked on the HyperOS 4 China ROM.**
An LSPosed module for the HyperOS 4 China ROM.

[Türkçe açıklama aşağıda](#türkçe)

## Why
The China ROM hides many features of the Security app: Game Turbo tools, the 60 FPS limit for games that are not on Xiaomi's list, battery health details, smart charging options, the full Toolbox and more. Modded Security APKs bring them back, but they replace a system app and break with every update.

XSecurity enables these features on the **stock** apps with LSPosed hooks. No system APK replacement is required, and each feature has its own switch. Compatibility depends on the ROM and app versions.

## Features
- 🎮 **Games:** remove the 60 FPS cap, Game Turbo tools (HDR, super resolution, frame interpolation, touch, extras), Wild Boost and performance modes.
- 🔋 **Battery & charging:** app battery ranking and screen-on time, battery health (capacity, cycles, temperature), charge-protection and smart-charging options, low-temperature endurance.
- 🌐 **Network:** keep mobile data on past the quota, keep the hotspot on, data usage in Control Center.
- 📱 **App info:** extra rows (version code, UID, data, APK path, target SDK) with tap to copy, plus Open in Play Store. The header has Open, Path and a chain-icon Open by default action; the duplicate lower action is removed.
- ⚙️ **System:** full global Toolbox, 50 apps in the sidebar, no permission countdown, video & call toolbox, second space, car accident / car sickness features, storage defragmentation (FBO).
- 🌙 **Dark mode:** list every installed app under "Individual apps" instead of just a few.
- 🏪 **App store:** show a chooser for `market://` links instead of forcing GetApps, and open GetApps detail pages in a floating window.
- 🔧 **Signature verification bypass:** 11 individual installation options, including signature compatibility, downgrades and persistent system app updates. These options do not migrate packages to a different shared UID.
- 📸 **Screenshot and screen recording:** optional removal of supported `FLAG_SECURE` and HyperOS capture restrictions.
- 📋 **Clipboard:** choose which apps may read the clipboard in the background.
- 🛡️ **Privacy:** optional prevention of app-list uploads by Xiaomi Guard Provider.
- 🎭 **Themes:** optional prevention of applied themes reverting to default.
- 📦 **System updater:** skip the "auto update" dialog and the OTA validation prompt (optional, off by default).
- 🎨 **App:** HyperOS (Miuix) or Material You look, light / dark / system theme, 5 languages, hide the home screen icon.

Most switches that change how the phone behaves are off by default; turn on what you want. Framework features need the **System Framework** scope and a reboot. Gallery integration has been removed in 1.5. Open XSecurity once after updating to clean up its retired preference and scope.

## Requirements
- A Xiaomi phone on the HyperOS 4 China ROM
- Root (KernelSU, SukiSU or Magisk) and LSPosed (API 102)

## Install
1. Install XSecurity.
2. Enable it in LSPosed and review the recommended scope: System Framework (`system`), Security (`com.miui.securitycenter`), Battery and performance (`com.miui.powerkeeper`), Updater (`com.android.updater`), Joyose (`com.xiaomi.joyose`), Themes (`com.android.thememanager`) and Guard Provider (`com.miui.guardprovider`).
3. Grant XSecurity its LSPosed permission, otherwise the app shows "Not active".
4. Reboot for the framework features.

## Source code and support
- Source: https://github.com/Leekin2/XSecurity (AGPL-3.0)
- Some hooks are re-implementations of [HyperCeiler](https://github.com/ReChronoRain/HyperCeiler) rules (AGPL-3.0); see NOTICE.
- Feedback: Telegram [@emcleek](https://t.me/emcleek) · group [Xgoogle for HyperOS](https://t.me/Xgooogle)

---

## Türkçe

**HyperOS 4 Çin ROM'unda bölgeye kilitli Güvenlik uygulaması özelliklerini açar.**
HyperOS 4 Çin ROM'u için bir LSPosed modülü.

### Neden
Çin ROM'u Güvenlik uygulamasının birçok özelliğini gizler: Game Turbo araçları, Xiaomi'nin listesinde olmayan oyunlar için 60 FPS sınırı, pil sağlığı ayrıntıları, akıllı şarj seçenekleri, tam Araç kutusu ve daha fazlası. Modlu Güvenlik APK'ları bunları geri getirir ama bir sistem uygulamasının yerine geçer ve her güncellemede bozulur.

XSecurity bu özellikleri LSPosed hook'larıyla **orijinal** uygulamalarda açar. Sistem APK'sını değiştirmek gerekmez ve her özelliğin kendi anahtarı vardır. Uyumluluk ROM ve uygulama sürümlerine bağlıdır.

### Özellikler
- 🎮 **Oyunlar:** 60 FPS sınırını kaldır, Game Turbo araçları (HDR, süper çözünürlük, kare ekleme, dokunma, ekstralar), Wild Boost ve performans modları.
- 🔋 **Pil ve şarj:** uygulama pil sıralaması ve ekran süresi, pil sağlığı (kapasite, döngü, sıcaklık), şarj koruması ve akıllı şarj seçenekleri, düşük sıcaklık dayanıklılığı.
- 🌐 **Ağ:** kota bitince mobil veri açık kalsın, hotspot açık kalsın, kontrol merkezinde veri kullanımı.
- 📱 **Uygulama bilgisi:** ek satırlar (sürüm kodu, UID, veri, APK yolu, hedef SDK), dokununca kopyala ve Play Store'da aç. Üstte Aç, Yol ve zincir simgeli Varsayılan aç bulunur; alttaki tekrar kaldırılmıştır.
- ⚙️ **Sistem:** global tam Araç kutusu, yan çubukta 50 uygulama, izin geri sayımı yok, video & arama araç kutusu, ikinci alan, kaza/araç tutması özellikleri, depolama birleştirme (FBO).
- 🌙 **Karanlık mod:** "Tek tek uygulamalar" altında birkaç uygulama yerine yüklü tüm uygulamalar.
- 🏪 **Uygulama mağazası:** `market://` bağlantılarında GetApps'e zorlamak yerine seçici göster, GetApps detaylarını kayan pencerede aç.
- 🔧 **İmza doğrulamasını atlama:** imza uyumluluğu, sürüm düşürme ve kalıcı sistem uygulamalarını güncelleme dahil 11 ayrı kurulum seçeneği. Bu seçenekler paketleri farklı bir ortak UID'ye taşımaz.
- 📸 **Ekran görüntüsü ve ekran kaydı:** desteklenen `FLAG_SECURE` ve HyperOS yakalama kısıtlamalarını kaldırma seçeneği.
- 📋 **Pano:** arka planda panoyu okuyabilecek uygulamaları seçme.
- 🛡️ **Gizlilik:** Xiaomi Guard Provider'ın uygulama listesi yüklemesini engelleme seçeneği.
- 🎭 **Temalar:** uygulanan temanın varsayılana dönmesini önleme seçeneği.
- 📦 **Sistem güncelleyici:** "otomatik güncelleme" diyaloğunu ve OTA doğrulama uyarısını atla (isteğe bağlı, varsayılan kapalı).
- 🎨 **Uygulama:** HyperOS (Miuix) veya Material You görünümü, açık / koyu / sistem teması, 5 dil, ana ekran simgesini gizle.

Telefonun davranışını değiştiren çoğu anahtar varsayılan kapalıdır; istediğini aç. Framework özellikleri için **System Framework** kapsamı ve yeniden başlatma gerekir. Galeri entegrasyonu 1.5 sürümünde kaldırıldı. Eski tercih ve kapsamı temizlemek için güncellemeden sonra XSecurity'yi bir kez açın.

### Gereksinimler
- HyperOS 4 Çin ROM'lu bir Xiaomi telefon
- Root (KernelSU, SukiSU veya Magisk) ve LSPosed (API 102)

### Kurulum
1. XSecurity'yi kurun.
2. LSPosed'da etkinleştirin ve önerilen kapsamı kontrol edin: Sistem Çerçevesi (`system`), Güvenlik (`com.miui.securitycenter`), Pil ve performans (`com.miui.powerkeeper`), Güncelleyici (`com.android.updater`), Joyose (`com.xiaomi.joyose`), Temalar (`com.android.thememanager`) ve Guard Provider (`com.miui.guardprovider`).
3. Modülün LSPosed iznini verin, yoksa uygulama "Etkin değil" gösterir.
4. Framework özellikleri için yeniden başlatın.

### Kaynak kod ve destek
- Kaynak: https://github.com/Leekin2/XSecurity (AGPL-3.0)
- Bazı hook'lar [HyperCeiler](https://github.com/ReChronoRain/HyperCeiler) kurallarının yeniden uyarlamasıdır (AGPL-3.0); bkz. NOTICE.
- Geri bildirim: Telegram [@emcleek](https://t.me/emcleek) · grup [Xgoogle for HyperOS](https://t.me/Xgooogle)
