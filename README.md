# Technická správa k projektu ITW: Osobné portfólio

**Autor:** Michal Senderák  
**Login:** xsendem00  
**URL projektu:** [https://miso125.github.io/itw-portfolio/](https://miso125.github.io/itw-portfolio/)

---

## 1. Popis a architektúra riešenia
Predmetom projektu je návrh a implementácia profilovej webovej prezentácie vo forme "Single Page" aplikácie. Architektúra riešenia je zameraná na čistý vizuálny štýl, responzivitu a dodržiavanie moderných webových štandardov.

Aplikácia je rozdelená do šiestich hlavných informačných sekcií, čím dostatočne popisuje referovanú osobu. Navigácia medzi sekciami je riešená prostredníctvom globálneho fixného navigačného panela s implementáciou plynulého prechodu (smooth scrolling).

## 2. Technická špecifikácia
Projekt je realizovaný výlučne pomocou natívnych technológií bez použitia externých CSS frameworkov (ako napr. Bootstrap), čím preukazuje porozumenie základným princípom.

* **Sémantické HTML5:** Kód je štruktúrovaný pomocou sémantických značiek (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`). Toto riešenie zabezpečuje logické členenie dokumentu, prístupnosť a plnú srozumiteľnosť obsahu aj bez podpory kaskádových štýlov. Výsledný kód bol overený W3C validátorom.
* **Kaskádové štýly (CSS3):**
  * **Layout:** Rozloženie obsahu je implementované kombináciou modulov **CSS Flexbox** (striedavé radenie prvkov, zarovnanie navigácie) a **CSS Grid** (responzívna mriežka v sekcii skúseností a "Bento Box" usporiadanie záujmov).
  * **Responzivita a adaptabilita:** Dizajn je plne responzívny s využitím `media queries` pre korektné zobrazenie na mobilných zariadeniach (vrátane implementácie "hamburger menu").
  * **Vizuálny štýl:** Bol navrhnutý konzistentný pastelový farebný koncept riadený pomocou CSS premenných. Súčasťou návrhu je implementácia efektu matného skla ("Glassmorphism") cez vlastnosť `backdrop-filter` a optimalizácia kontrastu textu na grafických pozadiach za pomoci vrstvenia a prechodov (linear-gradient).
  * **Mikrointerakcie:** Do užívateľského rozhrania boli integrované jemné CSS animácie a hover efekty pre zvýraznenie aktívnych prvkov (transformácie, tieňovanie).
* **JavaScript:** Využitý bol výlučne minimálny "Vanilla JS" kód pre riadenie stavov (otváranie/zatváranie) mobilného navigačného menu.

## 3. Využitie umelej inteligencie (AI)
Jazykové modely boli využívané prevažne ako všeobecne podporný nástroj pri návrhu, testovaní a vylaďovaní riešenia. Bol využívaný prevažne na objasnenie princípov, návrhy možných spôsobov štýlov a návrh originálneho riešenia.

**Oblasti asistencie AI:**
1. **Architektúra CSS:** Konzultácia matematických a syntaktických pravidiel pri návrhu asymetrického rozloženia (CSS Grid span) pre sekciu s vizuálnou galériou (Bento Box layout).
2. **Ladenie a optimalizácia (Debugging):** Detekcia a oprava anomálií pri vykresľovaní rôznorodých formátov obrázkov. Výsledkom bolo korektné nasadenie vlastností `aspect-ratio` a `object-fit` pre zachovanie geometrie kontajnerov.
3. **Generovanie CSS vzorov:** Asistencia pri návrhu kľúčových snímok (`@keyframes`) pre plynulé animácie pozadia a štruktúrovanie CSS prechodov (gradient text).



## 4. Štruktúra prezentácie
Webová prezentácia je vnútorne členená na nasledujúce sekcie:
1. **Úvod:** Identifikácia, primárne zameranie a hlavný nadpis fungujúci ako absolútny odkaz na umiestnenie webu.
2. **O mne:** Profilové informácie.
3. **Skúsenosti:** Technické a študijné zručnosti, obsahujúce vnútorné podsekcie (Vzdelanie, Technológie).
4. **Projekty:** Vizualizované ukážky technických prác.
5. **Záujmy:** Grafická sekcia doplnená o fotografie voľne dostupné na internete.
6. **Kontakt:** Odkazy na externé siete a komunikačné kanály.