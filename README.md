# 🎨 GLR Creative Coding Grid: The Collaborative Wall

**Welkom Developers.**

Vandaag bouwen we niet alleen. Vandaag bouwen we **samen**.
Dit project is een experiment in **massale samenwerking**. Met de hele klas werken we tegelijkertijd aan één webpagina: een interactieve "Muur" die zichzelf automatisch opbouwt.

Jouw doel? Jouw stukje van de muur claimen, stylen en publiceren zonder de boel voor de rest te slopen. 🚀

---

## ⚠️ De Gouden Regels (De Robot kijkt mee!)

We werken met een **automatische politieagent** (CI/CD Pipeline). Als je je niet aan de regels houdt, wordt je code **automatisch afgekeurd**.

1.  **🚫 GEEN `<html>`, `<head>` of `<body>` tags.**
    * Je bouwt een *onderdeel* (component), geen hele pagina.
2.  **🚫 GEEN `position: fixed`.**
    * Blijf in je eigen vakje.
3.  **🚫 GEEN Externe Plaatjes of Javascript.**
    * Geen `<img src="...">` en geen `background-image: url(...)`.
    * **Challenge:** Alles wat je ziet moet je zelf tekenen met CSS (shapes, gradients, borders)!
4.  **🔒 Blijf van de Systeembestanden af.**
    * Raak `index.html`, `style.css`, `script.js` en de `.github` map NIET aan. De "Watchdog" ziet alles! 👀
5.  **✍️ Werk ALLEEN in je eigen bestand.**
    * Je maakt een bestand aan met jouw eigen studentnummer.

---

## 🛠️ De Workflow

Volg deze stappen precies, anders ontstaan er conflicten (en huilende docenten).

### Stap 1: Setup
1.  **Clone** deze repository naar je laptop.
2.  Maak direct een **nieuwe branch** aan.
    * Naamgeving: `feature/jouw-naam` (bijv. `feature/piet-puk`).
    * *Werk nooit direct op de `main` branch!*

### Stap 2: Maak je bestand
1.  Ga naar de map `tiles/`.
2.  Kopieer het bestand `_template.html`.
3.  **Hernoem** de kopie naar jouw studentnummer.
    * *Voorbeeld:* `84592.html`
4.  Open jouw bestand en pas het ID in de CSS en HTML aan naar jouw nummer (bijv. `#tile-84592`).

### Stap 3: 🧪 Lokaal Testen (Belangrijk!)
De website weet nog niet dat jouw bestand bestaat. Draai het hulpscript om dit lokaal te fixen:

1.  Open de **Terminal** in VS Code (`Ctrl + ~`).
2.  Zorg dat je **Git Bash** gebruikt (selecteer via het pijltje naast de `+`).
3.  Typ het volgende commando en druk op Enter:
    ```bash
    ./generate-list.sh
    ```
4.  Open nu `index.html` in je browser. Je tegel staat erbij! 🎉

---

## 🚀 Missie 1: Hello World (De Eerste 20 Minuten)

**Doel:** Bewijzen dat je samen kunt werken met Git en GitHub.

1.  Zorg dat je vakje een **achtergrondkleur** heeft en dat **jouw naam** erin staat.
2.  Sla je bestand op.
3.  **Commit** je wijzigingen (bericht: *"Mijn tegel geclaimd"*).
4.  **Push** je branch naar GitHub.
5.  Ga naar GitHub.com en maak een **Pull Request (PR)** aan naar de `main` branch.
6.  **WACHT.**
    * Kijk naar de checks. Worden ze groen? ✅ → Top! De docent zal je mergen.
    * Worden ze rood? ❌ → Je hebt een regel overtreden. Fix het in je code, push opnieuw, en de check gaat weer lopen.

---

## 🎨 Missie 2: Make it Shine (Rest van de les)

**Doel:** Laat je CSS skills zien & Design for Detail.

Nu je tegel live staat, gaan we hem mooi maken.
* Gebruik `hover` effecten (dingen die bewegen als je muis erover gaat).
* Gebruik `transform`, `transition` of `border-radius`.

### 🔍 Bonus Missie: Design for Detail
Let op: Op het grote grid is je tegel vrij klein.
**MAAR...** als we erop klikken, wordt hij schermvullend (**Bioscoopmodus**)! 🍿

* **De Uitdaging:** Zorg dat je ontwerp er van veraf duidelijk uitziet (grote vormen/kleuren), maar verstop **kleine details** die we pas zien als we inzoomen.
* *Voorbeeld:* Een huisje is leuk van veraf. Maar als we inzoomen, zien we pas de kat in de vensterbank.

**Klaar?**
1.  Commit & Push opnieuw.
2.  Check je Pull Request (deze wordt automatisch geüpdatet).
3.  Wacht tot de docent je update merged op het grote scherm.

---

## 🆘 Help, mijn check faalt!

Krijg je een rood kruis bij je Pull Request? Klik op **"Details"**. De robot vertelt je precies wat er mis is.
* *"Forbidden Tags found"* → Je hebt per ongeluk `<html>` of `<body>` laten staan. Haal ze weg!
* *"Images not allowed"* → Je probeert een plaatje te gebruiken. Teken het na met CSS!
* *"System Files changed"* → Je hebt per ongeluk in `style.css` of `index.html` gewerkt. Draai die wijzigingen terug.

Succes! 💻✨