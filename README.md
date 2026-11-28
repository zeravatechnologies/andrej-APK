# APK — Android aplikacije · Android apps

Linkovi za preuzimanje svih Android aplikacija (APK) iz
[andrejristic](https://github.com/andrejristic) repoa. Lista se osvežava sama, svakog sata.

Download links for every Android app (APK) from the
[andrejristic](https://github.com/andrejristic) repositories. The list updates itself every hour.

<!-- APK-INDEX:START -->
| Aplikacija · App | Verzija · Version | Datum · Date | Preuzmi · Download |
|---|---|---|---|
| [attack_mapper](https://github.com/andrejristic/attack_mapper)<br><sub>Multi-turn attack-surface mapper: detect jailbreaks & attack patterns in AI conversations</sub> | v0.9.1-test | 2026-11-26 | test: [attack-mapper-0.9.1-test.apk](https://github.com/andrejristic/attack_mapper/releases/download/v0.9.1-test/attack-mapper-0.9.1-test.apk) |
| [pseek](https://github.com/andrejristic/pseek)<br><sub>PSE project: pseek</sub> | v0.1.0-test | 2026-11-28 | test: [pseek-0.1.0-test.apk](https://github.com/andrejristic/pseek/releases/download/v0.1.0-test/pseek-0.1.0-test.apk) |

<details><summary>Sve verzije · All builds</summary>

**attack_mapper**

- [attack-mapper-0.9.1-test.apk](https://github.com/andrejristic/attack_mapper/releases/download/v0.9.1-test/attack-mapper-0.9.1-test.apk) · v0.9.1-test _(test)_ · 2026-11-26 · 86.4 MB
- [attack-mapper-0.9.0-test-test.apk](https://github.com/andrejristic/attack_mapper/releases/download/v0.9.0-test/attack-mapper-0.9.0-test-test.apk) · v0.9.0-test _(test)_ · 2026-11-25 · 86.4 MB

**pseek**

- [pseek-0.1.0-test.apk](https://github.com/andrejristic/pseek/releases/download/v0.1.0-test/pseek-0.1.0-test.apk) · v0.1.0-test _(test)_ · 2026-11-28 · 72.6 MB

</details>
<!-- APK-INDEX:END -->

**Test** verzije su za probu pre zvaničnog izdanja. Mogu se instalirati pored zvanične verzije.
**Test** builds are previews; they install side by side with the official version.

---

## Kako instalirati (srpski)

### Android telefon ili tablet
1. Na telefonu otvori ovu stranicu i dodirni link za APK. Fajl se preuzima.
2. Otvori preuzeti fajl (obaveštenje „Preuzimanje završeno“ ili aplikacija **Fajlovi → Preuzimanja**).
3. Ako Android pita, dozvoli instalaciju: **Podešavanja → Instaliraj nepoznate aplikacije →**
   izaberi browser (npr. Chrome) **→ Dozvoli iz ovog izvora**. Vrati se nazad i dodirni **Instaliraj**.
4. Ako se pojavi Google Play Protect upozorenje, izaberi **Više detalja → Ipak instaliraj**
   (aplikacija još nije na Google Play-u, pa je Play ne poznaje).

### Chromebook
1. Uključi Android aplikacije: **Podešavanja → Aplikacije → Google Play prodavnica → Uključi**.
2. **Probaj prvo ovo:** iz Play prodavnice instaliraj Android menadžer fajlova (npr. „Files by Google“),
   preuzmi APK i otvori ga iz te aplikacije. Ako Android pita za dozvolu
   „Instaliraj nepoznate aplikacije“, dozvoli je za tu aplikaciju. Na nekim modelima ovo radi odmah.
3. **Zvanični put (uvek radi):** ADB iz Linuxa. ⚠️ **Prvo uključivanje ADB-a na Chromebooku traži
   Powerwash, to jest brisanje svih lokalnih podataka.** Prvo napravi rezervnu kopiju.
   **Podešavanja → Napredno → Programeri → Linux razvojno okruženje → Uključi**, pa
   **Razvoj Android aplikacija → Omogući ADB otklanjanje grešaka**. Posle restarta, u Linux terminalu:
   `sudo apt install adb`, pa `adb install "<ime-fajla>.apk"` (APK prvo prevuci u **Linux fajlove**).
4. Ako ti brisanje ne odgovara, testiraj na Android telefonu (gore). Tamo je najlakše.

## How to install (English)

### Android phone or tablet
1. Open this page on the phone and tap the APK link to download it.
2. Open the downloaded file (the "Download complete" notification or **Files → Downloads**).
3. If Android asks, allow installs: **Settings → Install unknown apps →** your browser
   **→ Allow from this source**, go back and tap **Install**.
4. If Google Play Protect warns you, choose **More details → Install anyway**
   (the app is not on Google Play yet, so Play does not know it).

### Chromebook
1. Turn on Android apps: **Settings → Apps → Google Play Store → Turn on**.
2. **Try this first:** install an Android file manager from the Play Store (e.g. "Files by Google"),
   download the APK and open it from that app. If Android asks for "Install unknown apps",
   allow it for that app. On some models this works right away.
3. **Official way (always works):** ADB from Linux. ⚠️ **Turning ADB on for the first time on a
   Chromebook requires a Powerwash, which erases all local data.** Back up first.
   **Settings → Advanced → Developers → Linux development environment → Turn on**, then
   **Develop Android apps → Enable ADB debugging**. After the restart, in the Linux terminal:
   `sudo apt install adb`, then `adb install "<file>.apk"` (move the APK into **Linux files** first).
4. If erasing is not an option, test on an Android phone (above); that is the easiest.

---

Kako funkcioniše · How it works: [`scripts/update_index.py`](scripts/update_index.py) prolazi kroz
javne repoe, nalazi GitHub Releases sa `.apk` fajlovima i upisuje linkove ovde
([`.github/workflows/update-index.yml`](.github/workflows/update-index.yml)).
APK fajlovi se ne čuvaju u ovom repou nego u Releases svake aplikacije.
