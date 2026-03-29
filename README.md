# AurealisRemote

Webové ovládání pro WLED zařízení **Aurealis** - chytré LED osvětlení s ovládáním přes WiFi.

## 🚀 Rychlý start

### Postup použití:

1. **Otevřete webovou stránku** na GitHubu
   - Otevřete URL: `https://susiox.github.io/AurealisRemote/AurealisRemote.html`
   - Stránka se načte (zatím není aktivní)

2. **Připojte se k WiFi sítě "Aurealis"**
   - Tuto síť vysílá přímo WLED zařízení (ESP32/ESP8266)
   - Na mobilu/PC vyhledejte WiFi síť **"Aurealis"**
   - Připojte se (bez hesla, nebo s heslem které jste nastavili)
   - WLED má v AP módu IP adresu: **4.3.2.1**

3. **Ovládejte LED**
   - Nyní stránka komunikuje přímo s WLED
   - Klikání na tlačítka okamžitě mění barvy a efekty

## 🎨 Dostupné režimy

| Tlačítko | Popis |
|-----------|-------|
| TMA | Tmavý režim (vypnuto) |
| Oranžová | Oranžová barva |
| Slunce | Sluneční světlo |
| Červená | Červená barva |
| Zelená | Zelená barva |
| Modrá | Modrá barva |
| Amber | Jantarová barva |
| Barvení | Náhodné barevné přechody |
| Duha | Duhový efekt |

## ⚙️ Konfigurace

### IP adresa
WLED v AP módu používá IP: **4.3.2.1**

### Presety
Presety jsou uloženy přímo ve WLED zařízení:
- Preset 1: TMA
- Preset 4: Slunce
- Preset 5: Oranžová
- Preset 101-108: Barvy a efekty

## 📱 Mobilní použití

Tato stránka je optimalizována pro mobilní telefony:
- Velké tlačítka pro snadné ovládání prsty
- Rychlá odezva
- Možnost použití offline (stažený soubor)

## 🔧 Technické detaily

- **Komunikace**: HTTP API (WLED API)
- **Metoda**: GET požadavky přes `new Image().src` (bez CORS problémů)
- **Formát**: HTML + CSS + JavaScript (bez externích závislostí)

## 📝 Poznámky

- Transition time je uložen přímo v WLED presety, není možné měnit z webu
- Pro plynulou změnu rychlosti se používá throttling (odeslání až po uvolnění slideru)

## 📄 Licence

MIT License - volně použitelné a modifikovatelné.

---

**Vytvořeno pro**: WLED projekt s názvem "Aurealis"
