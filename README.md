# Raport Endoskopie

Gjenerator raportesh për **gastroskopi (EGD)**, **kolonoskopi** ose **të dyja në të njëjtën seancë**, në shqip. Funksionon **offline** në iPad, kompjuter dhe telefon.

**Hape këtu:** https://doctorls.github.io/Gastroscopy/

## Instalimi në iPad
1. Hap adresën më sipër në **Safari**.
2. Shtyp **Share (⬆)** → **Add to Home Screen** → **Add**.
3. Hape gjithmonë nga ikona në ekranin kryesor. Pas hapjes së parë punon edhe pa internet.

> Aplikacioni në ekranin kryesor e ka arkivin e vet, të ndarë nga Safari. Përdor gjithmonë ikonën.

## Privatësia
- Të dhënat e pacientëve ruhen **vetëm në pajisjen tënde** (IndexedDB). Asgjë nuk dërgohet në internet.
- Ky repo përmban vetëm kodin e aplikacionit, pa asnjë të dhënë pacienti.

## Backup
- **Arkivi → Backup i plotë** krijon një skedar me të gjithë pacientët dhe fotot. Skedari mund të enkriptohet me fjalëkalim (AES-256).
- Në iPad zgjidh **Save to Files → iCloud Drive**. Bëje të paktën një herë në javë.
- **Rikthe nga backup** i sjell pacientët në një pajisje të re.
- ⚠ Fjalëkalimi i harruar nuk mund të rikthehet.

## Funksionet
- Gastroskopi: LA, Praga (Barrett), Forrest, Hill, Paris, varice F1–F3, biopsi sipas Sydney
- Kolonoskopi: shkalla e Bostonit (BBPS), intubimi cekal, koha e tërheqjes, tabela e polipeve (Paris, NICE, teknika e heqjes, kavanoza), divertikuj, hemoroide, kolit (Mayo, shtrirja)
- Raport i përbashkët kur bëhen të dyja procedurat
- Logoja dhe të dhënat e klinikës (⚙ Klinika) në krye të çdo raporti
- Konkluzion automatik nga gjetjet, rekomandime me një klik
- Foto endoskopike (edhe nga kamera e iPad-it)
- Printim / PDF në format A4 me logon e klinikës
- Temë e çelët / e errët

## Struktura
| Skedari | Roli |
|---|---|
| `index.html` | I gjithë aplikacioni (HTML + CSS + JS) |
| `sw.js` | Ruajtja offline e aplikacionit |
| `manifest.webmanifest` | Emri dhe ikonat për instalimin |
| `icons/` | Ikonat e aplikacionit |
