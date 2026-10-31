---
marp: true
paginate: true
style: |
  /* ==============================================================
     Vorlage für Marp
     Diese Datei ist dein Gerüst. Ändere Werte, niemals die Namen
     der Klassen – die müssen zum Text passen, sonst passiert nichts.

     Wichtig: Diese Vorlage nutzt HTML (<div class="...">). Marp
     blockiert das standardmäßig. Aktiviere HTML:
       - VS Code: Einstellung "markdown.marp.enableHtml"
       - Marp CLI: Option --html
     ============================================================== */

  /* --- Die Farben ------------------------------------------------
     Jede Farbe steht genau einmal hier. Alle Klassen weiter unten
     benutzen nur noch den Namen. Willst du das Aussehen ändern,
     änderst du nur diese sieben Zeilen – nicht die Klassen. */

  :root {
    --blau:      #17324d;   /* Titel, Balken, Linien */
    --blau-hell: #24527a;   /* Akzente, Rand der Karten */
    --flaeche:   #f7f9fc;   /* Hintergründe von Kästen */
    --flaeche-2: #edf5fb;   /* zweiter Hintergrundton */
    --flaeche-3: #e8f1f8;   /* dritter Hintergrundton */
    --flaeche-4: #eef5f9;   /* Karten */
    --gelb:      #f4d35e;   /* Hervorhebung */
  }

  /* --- Die Folie selbst ------------------------------------------
     Jede Folie wird zu einem <section>. Alles hier gilt für alle. */
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100%;
    padding: 40px;
    font-family: Arial, Helvetica, sans-serif;
  }

  /* --- Der Folientitel ------------------------------------------- */
  .titel {
    width: 100%;
    text-align: center;
    color: var(--blau);
    margin-bottom: 24px;
  }

  /* --- Eine einfache Liste --------------------------------------- */
  .liste {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Ein hervorgehobener Satz ---------------------------------- */
  .merksatz {
    width: 80%;
    margin-bottom: 20px;
    padding: 20px;
    background: var(--gelb);
    font-weight: bold;
    border-radius: 20px;
    text-align: left;
  }

  /* --- Ein einzelner Kasten -------------------------------------- */
  .box {
    width: 80%;
    padding: 18px 24px;
    background: var(--flaeche-2);
    border-left: 6px solid var(--blau);
    text-align: left;
  }

  /* --- Zwei Spalten: legt die Aufteilung fest -------------------- */
  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    width: 100%;
  }

  /* Spaltenverhältnisse zum Ausprobieren:
       1fr 1fr  -> zwei gleich breite Spalten
       2fr 1fr  -> links doppelt so breit wie rechts
       1fr 2fr  -> rechts doppelt so breit wie links               */

  /* Eine breite und eine schmale Spalte:
     .grid-2 { grid-template-columns: 2fr 1fr; align-items: center; } */

  /* --- Die Spalte: nur das Aussehen ------------------------------ */
  .spalte {
    padding: 18px;
    background: var(--flaeche-3);
    border-radius: 14px;
    text-align: left;
  }

  /* --- Karten: drei Dinge nebeneinander -------------------------- */
  .karten {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
    width: 100%;
  }

  .karte {
    min-height: 150px;
    padding: 16px;
    background: var(--flaeche-4);
    border-top: 5px solid var(--blau-hell);
    text-align: left;
  }

  /* --- Bilder ---------------------------------------------------- */
  .bild {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
  }

  .bild img {
    width: 320px;
    height: auto;
  }

  /* --- Die Fußzeile ---------------------------------------------- */
  .fusszeile {
    width: 100%;
    margin-top: auto;
    padding-top: 12px;
    border-top: 1px solid var(--blau);
    text-align: center;
    font-size: 0.6em;
  }
---

<div class="titel">

# Welcher Passwortmanager ist die Beste option für den Preis?

</div>

<div class="liste">



- Ziyu Fan
- 9c
- 2.11.26

</div>

<div class="fusszeile">
  Passwortmanager · Ziyu Fan, 9c
</div>

---

<div class="titel">

# Welche Punkte sind mir wichtig in einem Passwortmanager

</div>

<div class="liste">

- Preis
- Zero Knowledge Sicherheit
- Passwortgenerator

</div>

<div class="fusszeile">
  Welche Punkte sind mir wichtig in einem Passwortmanager · Ziyu Fan, 9c
</div>

---

<div class="titel">

# Die Punkte Erklärt

</div>

<div class="karten">
  <div class="karte">

  **Preis**

  - Wie viel der Passwortmanager Kostet
  - Was man alles bekommt für den Preis

  </div>
  <div class="karte">

  **Zero Knowledge Sicherheitr**

  - Das die Passwörter local verschlüsselt werden
  - Das die Anbieter / der Passwortmanager kein zugriff auf 

  

  </div>
  <div class="karte">

  **Passwortgenerator**

  - Gute Passwörter einfach generieren können.

 </div>
</div>

<div class="fusszeile">
  Überblick · Ziyu Fan, 9c
</div>

---

<div class="titel">

# Bekannte Passwortmanager

</div>

<div class="liste">

- Bitwarden
- Keeper
- Nordpass

</div>

<div class="fusszeile">
 Bekannte Passwortmanager · Ziyu Fan, 9c
</div>

---

<div class="titel">

# Drei Dienste im Überblick

</div>

<div class="karten">
  <div class="karte">

  **Bitwarden**

  - kostenlos mit Zusatzangeboten
  - Quellcode: Open Source
  - Unterschied: Billigste Option

  </div>
  <div class="karte">

  **Keeper**

  - kostenlos mit Zusatzangeboten
  - Quellcode: Nicht Open Source
  - Unterschied: Dark-Web Monitoring

  </div>
  <div class="karte">

  **Nordpass**

  -  kostenlos mit Zusatzangeboten
  - Quellcode: Nicht Open Source
  - Unterschied: Benutzt das beste Verschlüsselungsalgorithmus

  </div>
</div>

<div class="fusszeile">
  Überblick · Ziyu Fan, 9c
</div>

---



<div class="titel">

# Fazit

</div>

<div class="liste">

- Bitwarden ist die Beste option
- Billigste option
- Open Source
- Viele Funktionen
- Kostenlos
</div>

<div class="fusszeile">
  Fazit · Ziyu Fan, 9c
</div>

---



<div class="titel">

# Danke für ihre Aufmerksamkeit

</div>




</div>

<div class="fusszeile">
  Fazit · Ziyu Fan, 9c
</div>

---
<div class="titel">

# Quellen

</div>

<div class="liste">

- [Funktionen die man in einem Passwortmanager suchen sollte](https://www.keepersecurity.com/blog/de/2025/07/18/8-features-to-look-for-in-a-password-manager/), abgerufen am 26.10.26
- [Wie erstellt man ein sicheres Passwort](https://www.bsi.bund.de/DE/Themen/Verbraucherinnen-und-Verbraucher/Informationen-und-Empfehlungen/Cyber-Sicherheitsempfehlungen/Accountschutz/Sichere-Passwoerter-erstellen/sichere-passwoerter-erstellen_node.html), abgerufen am 26.MM.JJ
- [Warum man ein Passwortgenerator nutzen sollte](https://www.keepersecurity.com/blog/de/2022/11/30/why-you-should-use-a-random-password-generator/), abgerufen am 26.10.26
- [Keeper Funktionen]( https://www.keepersecurity.com/de_DE/free-trial-vs-free-version.html ), abgerufen am 27.10.26
- [Keeper preise](https://www.keepersecurity.com/de_DE/pricing/personal-and-family.html), abgerufen am 27.10.26
- [Keeper Breachwatch](https://www.keepersecurity.com/de_DE/personal-breachwatch.html), abgerufen am 27.10.26
- [Bitwardens Source code](https://github.com/bitwarden), abgerufen am 27.10.26




</div>

<div class="fusszeile">
  Quellen · Ziyu Fan, 9c
</div>

---

<div class="titel">

# Quellen

</div>

<div class="liste">

- [Bitwardens Preise]( https://bitwarden.com/de-de/products/personal/), abgerufen am 27.10.26
- [Nordpass Preise](https://nordpass.com/de/password-manager/  ), abgerufen am 29.10.26
- [Nordpass Verschlüsselung](https://nordpass.com/de/features/xchacha20-encryption/ ), abgerufen am 29.10.26






</div>

<div class="fusszeile">
  Quellen · Ziyu Fan, 9c
</div>
