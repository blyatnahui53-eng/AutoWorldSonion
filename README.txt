Grundlagen und Basis von HTML und CSS
Das Fundament jeder Website im World Wide Web basiert auf dem perfekten Zusammenspiel zweier Kernsprachen: HTML und CSS.

HTML (HyperText Markup Language) bildet das strukturelle Skelett einer Webseite. Es ist keine klassische Programmiersprache, sondern eine Auszeichnungssprache (Markup Language). Mit HTML teilst du dem Browser mit, welche Inhalte auf der Seite vorhanden sein sollen und welche Rolle sie einnehmen. Das geschieht über sogenannte Tags (wie Überschriften <h1>, Absätze <p>, Listen <ul> oder Bilder <img>). HTML definiert also den reinen Inhalt und die logische Hierarchie – vergleichbar mit den Wänden und der Raumaufteilung eines Rohbaus.

CSS (Cascading Style Sheets) ist hingegen für das Aussehen, das Design und das Layout zuständig. Während HTML festlegt, was da ist, bestimmt CSS, wie es aussieht. Mit CSS steuerst du Farben, Schriftarten, Abstände, Hintergründe, Animationen und komplexe Anordnungen (wie Grid- oder Flexbox-Layouts). Das Besondere an CSS ist das Prinzip der „Kaskade“: Stile vererben sich oder überschreiben sich nach bestimmten Prioritätsregeln, was eine zentrale und effiziente Gestaltung der gesamten Website ermöglicht.

Zusammenfassend lässt sich sagen: HTML liefert den Inhalt und die Struktur, während CSS das Design und die visuelle Präsentation übernimmt. Erst durch die Kombination entsteht eine moderne, ansprechende Website.

Aufbau der „AutoWorld“-Beispielwebsite
Der Quelltext deines Beispiels zeigt eine typische, professionell strukturierte Website, die aus einem HTML-Dokument (dem Grundgerüst) und einem Ausschnitt eines CSS-Stylesheets (dem Design) besteht. Der Aufbau lässt sich in folgende Bereiche gliedern:

1. Der HTML-Kopf (<head>) und die Metadaten
Am Anfang des HTML-Codes definiert <!DOCTYPE html> den modernen HTML5-Standard. Das <html>-Tag mit dem Attribut lang="de" legt fest, dass die Sprache der Website Deutsch ist.

Im <head>-Bereich befinden sich unsichtbare Steuerinformationen für den Browser und Suchmaschinen: Der Zeichensatz (UTF-8), die Skalierbarkeit für mobile Geräte (viewport) sowie eine Meta-Beschreibung für Suchmaschinen.

Der Titel <title> bestimmt den Text, der im Browserreiter angezeigt wird („AutoWorld – Die Welt der Automobile“).

Über das <link>-Tag wird die externe CSS-Datei (style.css) eingebunden, die das gesamte Design der Seite steuert.

2. Der sichtbare Inhalt (<body>)
Der Hauptinhalt der Website ist in zwei große semantische Bereiche unterteilt: den Header und den Main-Bereich.

Der Header & Hero-Bereich (<header class="hero">):
Dieser obere, bildgewaltige Einstiegsbereich dient als Aushängeschild der Website. Er enthält die Navigation (<nav>) mit dem Logo und Links zu den verschiedenen Unterkapiteln (wie Grundlagen, Fahrzeugtypen oder Rennsport). Darunter folgt der eigentliche „Hero-Inhalt“ mit einer Eyebrow-Zeile, einer markanten Hauptüberschrift (<h1>), Beschreibungstexten, Call-to-Action-Buttons sowie kleinen Statistik-Boxen. Auch ein visueller Bereich mit einem Platzhalterbild (images/car-hero.jpg) und einer Themen-Leiste (topic-bar) ist hier integriert.

Der Hauptbereich (<main>):
Der <main>-Container umschließt die inhaltlichen Kernsektionen der Website. Jedes Thema ist als eigener <section>-Block mit einer klaren ID (z. B. id="grundlagen", id="fahrzeugtypen", id="antrieb") aufgebaut. Das ermöglicht es, dass die Navigationslinks direkt zu diesen Abschnitten springen. Innerhalb dieser Sektionen kommen diverse HTML-Elemente zum Einsatz:

Zweispaltige Layouts und Info-Karten für Definitionen.

Listen (<ul>, <li>) zur Aufzählung von Fahrzeugtypen oder Sicherheitsmerkmalen.

Tabellen (<table>, <thead>, <tbody>) beim Antriebssystem, um Vergleiche übersichtlich darzustellen.

Grid-Container und Cards (z. B. für berühmte Autos wie den Ferrari F40, den Ford Mustang oder den VW Käfer), um Inhalte in Rasterform anzuordnen.

3. Das CSS-Design (:root und Styles)
Im unteren Teil deines Codes beginnt das CSS, das für das Aussehen der oben beschriebenen Elemente sorgt:

CSS-Variablen (:root): Hier werden zentrale Farbpaletten (wie verschiedene Grüntöne für Akzente, dunkle Hintergrundfarben und neutrale Grautöne), Schatteneffekte (shadow-sm, shadow-md), Schriftarten und Übergangsgeschwindigkeiten definiert. Das hat den Vorteil, dass man Farben zentral an einer Stelle ändern kann und sie sich im gesamten Dokument anpassen.

Globaler Reset (*): Mit margin: 0; padding: 0; box-sizing: border-box; werden die Standardabstände des Browsers zurückgesetzt, damit das Design auf allen Geräten einheitlich berechnet wird.

Grundformatierung (html, body): Hier wird ein weiches Scrollen (scroll-behavior: smooth) aktiviert, die globale Textfarbe, die Hintergrundfarbe sowie die Standard-Schriftart für den Fließtext festgelegt.

Komponenten-Styling: Spezielle Klassen wie .navbar oder .logo sorgen dafür, dass die Navigation flexibel (display: flex), zentriert und optisch ansprechend (mit Farbverläufen) dargestellt wird.

Insgesamt zeigt dieser Code eine saubere, moderne und modulare Web-Architektur, bei der Struktur (HTML) und Gestaltung (CSS) strikt voneinander getrennt sind.