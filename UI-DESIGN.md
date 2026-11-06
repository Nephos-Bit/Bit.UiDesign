# Operative UI-Designsprache

Gestalte ruhig, präzise und einsatzorientiert. Information, Ort und Zustand stehen vor Dekoration.

- Komposition: Eine Hauptaufgabe pro Ansicht. Karte oder Lageinformation ist die dominante Fläche; Werkzeuge bleiben am Rand. Nutze Vollflächen mit Safe Areas statt schwebender Kartenraster.
- Hierarchie: Zeige kritischen Zustand und primäre Kennzahl zuerst, unterstützende Kontextwerte danach. Nutze kleine Versalien für Rubriken, klare metrische Zahlen und zurückhaltende Sekundärtexte.
- Flächen: Neutrale Flächen dominieren. Verwende transparente oder leicht getönte Overlays über Karte/Bild und feine Divider statt sichtbarer Rahmen. Vollständig deckende Flächen nur für fokussierte Formulare, Bestätigungen oder Listen.
- Farbe: Definiere semantische Tokens für Grundfläche, Primär-/Sekundärtext, Marke sowie Warnung und Fehler. Nutze höchstens einen Markenakzent pro Ansicht; Statusfarben tragen ausschließlich Statusbedeutung.
- Verläufe und Unschärfe: Verläufe dürfen nur leise eine Overlay-Kante in die Karte überführen. Unschärfe ist auf situative Header oder Werkzeugleisten begrenzt und darf Kontrast oder Kartenlesbarkeit nicht mindern. Keine dekorativen Schatten oder Verläufe.
- Typografie: Nutze eine technische, gut lesbare Sans-/Monospace-Kombination sparsam. Zahlen erhalten tabellarische Ziffern. Vermeide unnötige Fettschrift, Großüberschriften und lange Textblöcke in Lageansichten.
- Interaktion: Jede Touchaktion misst mindestens 44×44 px, besitzt Tastaturzugang, sichtbaren Fokus und einen erklärten Deaktivierungsgrund. Icon-only-Aktionen brauchen einen zugänglichen Namen.
- Bewegung: Übergänge dienen nur der Orientierung, bleiben kurz und respektieren reduzierte Bewegung. Kontinuierliche Livewerte wie Position, Kurs, Lage und Diagramme werden zwischen gültigen Zeitstempeln zeitbasiert interpoliert, damit die Darstellung flüssig bleibt; Zustandswechsel und Warnungen werden nie interpoliert. Timer, Sensoren und Animationen laufen nur für sichtbare, aktive Flächen.
- Themen: Jede neue Fläche wird für Dunkel, Hell und Automatik entwickelt. Neutralflächen bleiben dominant; Kontrast und Zustandsbedeutung müssen in allen Themes erhalten bleiben.
- Operationalität: Zeige live, veraltet, nicht verfügbar und fehlgeschlagen unterscheidbar. Teile Positionen nur validiert und mit verfügbarer Genauigkeit, Zeit und Kontext.
- Prüfung: Prüfe pro Erweiterung beide Themes, kleinen Touchscreen, Tastaturfokus, Offline-/Fehlerzustand und `prefers-reduced-motion`.
