# Projekt 1

28.8 bis 18.09

## Grob-Planung

Ich mache einen Website über mich (Personal Portfolio Website). Ich brauche ihn für meine Modelling-Karierre. 
Der Website soll aus mehreren Bereichen bestehen ("Home", "About", "Modeling", "Dance", "IT" und "Contact")

## 28.8.2026
Ziele:
- [x] Struktur der Website planen (welche Bereiche die Website haben soll)
- [x] Projekt vorbereiten (Github Repository)
- [x] HTML Grundstruktur erstellen (erste Bereiche der Website einfügen)
- [x] Design mit CSS beginnen (Schriftarten, Farben, Positionen bestimmen)

Gemacht:
- Struktur geplant und Bereiche ("Home", "About", "Modeling", "Dance", "IT", "Contact");
''' <nav class="navbar">
    <div class="logo">Daria</div>

    <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#modeling">Modeling</a>
        <a href="#dance">Dance</a>
        <a href="#it">IT</a>
        <a href="#contact">Contact</a>
    </div>
</nav> '''
(Startseite mit meinem Namen und kurzen Beschreibung erstellt);

- Github Repository;
  
- HTML, CSS und Java Grundstruktur erstellt ('index.html', 'style.css', 'script.js');
  
- CSS mit HTML verbunden (<link rel="stylesheet" href="style.css">) ;
  
- JavaScript Datei verbunden (<script src="script.js"></script>);
  
- Schriftarten (Arial, sans-serif), Farben (#f7f7f7 (hell grau) und #fafafa (weiss))
  Positionen
 ''' .hero {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}'''


## 4.9.2026
Ziele:
- [x] Inhalte vorbereiten (kurze texte schreiben, Bilder suchen);
- [x] HTML Bereich "About me" erstellen;
- [X] Bilder einfügen;
- [X] Design mit CSS verbessern (einheitliches Design, Bilder passend darstellen etc);
- [X] Website testen, Fehler korrigieren.

Gemacht:
- "About me" Bereich erstellt;
- Text über mich eingefügt;
- Ein eigenes Bild in die Website eingebaut
   '''<div class="about-image">
    <img src="IFSR26_14.jpg" alt="Photo of Daria">
</div>'''

  Wichtige Fehler bei mir:
  Falsch:
 ''' <div class="about-image">
</div>

<img src="IFSR26_14.jpg" alt="Photo of Daria">'''
  
Das Bild zuerst falsch eingebaut, weil der "img" Tag war ausserhalb von ".about-image", deshalb funktionierten die CSS Regeln für das Bild nicht. 

Korrigiert:
'''<div class="about-image">
    <img src="IFSR26_14.jpg" alt="Photo of Daria">
</div>'''


- Bildgrösse und Darstellung angepasst:
 ''' .about-image {
    width: 320px;
    height: 500px;
}

.about-image img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}'''

- Layout für "About Me" mit Flexbox erstellt:
 ''' .about-container {
    max-width: 1100px;
    width: 100%;
    margin: 0 auto;

    display: flex;
    gap: 50px;
    align-items: center;
    justify-content: center;
}'''

- Passende Darstellung für Handys begonnen:
 ''' @media (max-width: 786px) {
    .about-container {
        flex-direction: column;
        gap: 40px;
    }
}'''
Dadurch werden Text und Bilder auf kleinen Bildschirmen untereinander angezeigt. 

## 11.09.2026
Ziele:
- [x] Website mit Github Pages veröffentlichen;
- [x] Darstellung für Handys testen;
- [x] Modeling Bereich beginnen;
- [x] Galerie für "Modeling" vorbereiten.

Gemacht:
- Website mit Github pages veröffentlicht; Dabei gelernt, dass die Hauptdatei 'index.html' heissen muss und dass Dateipfade auf GitHub korrekt sein müssen. 
- Einen Fehler mit dem Bildpfad gefunden
  '''<img src="images/IFSR26_14.jpg">''' funktioniert nur, wenn das Bild wirklich im Ordner images liegt. Da mein Bild direkt neben index.html liegt verwende ich:
  '''<img src="IFSR26_14.jpg" alt="Photo of Daria">'''

- Navigation, Schriftgrössen und Layout für kleinere Bildschirme angepasst

 ''' @media (max-width: 786px) {

    .navbar {
        padding: 20px;
        flex-direction: column;
        gap: 15px;
    }

    .hero h1 {
        font-size: 42px;
    }

    .about-container {
        flex-direction: column;
    }

}'''


- Modeling Bereich erstellt und dabei einen html Fehler gefunden
  Falsch: </section class="modeling" id="modeling">
  Das war falsch, weil ein schliessender </section> Tag keine Klasse oder ID bekommt. 

  Korrekt: 
'''</section>
<section class="modeling" id="modeling">'''

Danach konnte die Website wieder normal nach unten gescrollt werden. 


- Galerie für 'Modeling' vorbereitet.


## 18.09
Ziele:
[] Modeling Galerie mit Bilder füllen;
[] Modeling Bereich optisch verbessern;
[] Dance Bereich erstellen;
[] Erste Java Script Funktion einbauen;
[] Navigation und Scroll Verhalten verbessern;
[] Fehler korrigieren

Gemacht zu Hause am 11.09:
- Drei einfache Modeling Bilder in die Gallerie einfügen:
 ''' <div class="modeling-gallery">
    <img src="model1.jpg" alt="Modeling photo">
    <img src="model2.jpg" alt="Modeling photo">
    <img src="model3.jpg" alt="Modeling photo">
</div>'''

- Bilder mit CSS einheitlich darstellen
      


