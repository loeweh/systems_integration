### Teil 1: Sehen in der Biologie und Mensch-Maschine-Schnittstelle

**Frage 1 (Berechnung)**

Um welchen Faktor verändert sich der subjektive Sinneseindruck der Helligkeit nach dem Weber-Fechner-Gesetz, wenn die absolute Reizstärke einer Lichtquelle von 15 cd auf 60 cd erhöht wird?

**Lösung:**

Nach dem Weber-Fechner-Gesetz ist die Empfindungsstärke $E$ proportional zum Logarithmus des Reizes $R$. Die Formel lautet:
$E = c \cdot \ln\frac{R}{R_{0}}$

Um den Faktor der Veränderung zu berechnen, kann die Differenz der Empfindungsstärken berechnet werden:
$\Delta E = E_{2} - E_{1} = c \cdot (\ln\frac{R_2}{R_0} - \ln\frac{R_1}{R_0}) = c \cdot \ln\frac{R_2}{R_1}$

Der Faktor ist somit der Logarithmus des Verhältnisses der beiden Reizstärken:
Faktor = $\ln(\frac{60}{15}) = \ln(4) \approx 1.386$

Der Sinneseindruck der Helligkeit verändert sich also um den Faktor 1,39.

---

**Frage 2 (Wissensfrage)**

Nennen Sie die 3 Komponenten des GOMS-Modells (ohne "Goals") und geben Sie die jeweilige durchschnittliche Zeitdauer für die Ausführung an.

**Lösung:**
[cite_start]Die 3 Komponenten des GOMS-Modells und ihre durchschnittlichen Zeitdauern sind[cite: 2190, 2195]:

* **Operators (Operatoren):**
    * [cite_start]**Keying (Tastatureingabe):** 0,2 Sekunden[cite: 2195].
    * [cite_start]**Pointing (Mauszeigen):** 1,1 Sekunden[cite: 2195].
    * [cite_start]**Homing (Wechsel Maus-Tastatur):** 0,4 Sekunden[cite: 2195].
    * [cite_start]**Mentally prepare (Vorbereiten):** 1,35 Sekunden[cite: 2195].
    * [cite_start]**Responding (Warten):** n Sekunden[cite: 2195].
* [cite_start]**Methods (Methoden):** Eine Folge von Operatoren, um ein Ziel zu erreichen[cite: 2189].
* [cite_start]**Selection Rules (Auswahlregeln):** Regeln, die festlegen, welche Methode gewählt wird, wenn mehrere zum Ziel führen[cite: 2189].

---

**Frage 3 (Berechnung)**

Wie lange dauert es laut Fitts'schem Gesetz, mit der Maus ein 20 Pixel breites Ziel anzuvisieren, das 400 Pixel vom Mauscursor entfernt ist? Verwenden Sie die in der Vorlesung angegebenen Konstanten.

**Lösung:**
Die Formel für das Fitt'sche Gesetz lautet:
[cite_start]$T = a + b \cdot Id(\frac{D}{S} + 1)$, wobei $Id = \log_2$[cite: 2150].

Gegebene Werte:
* Distanz $D = 400$ Pixel
* Größe des Ziels $S = 20$ Pixel
* [cite_start]Konstante $a = 50$ ms [cite: 2151]
* [cite_start]Konstante $b = 150$ ms [cite: 2151]

Berechnung:
1.  Verhältnis berechnen: $\frac{D}{S} + 1 = \frac{400}{20} + 1 = 20 + 1 = 21$
2.  Logarithmus dualis berechnen: $Id(21) = \log_2(21) \approx 4.392$
3.  In die Formel einsetzen: $T = 50 \text{ ms} + 150 \text{ ms} \cdot 4.392$
4.  Ausrechnen: $T \approx 50 + 658.8 = 708.8$ ms

Es dauert ungefähr **709 ms**.

---

**Frage 4 (Wissensfrage)**

Nennen Sie 3 wesentliche Unterschiede zwischen den Sehzellen Stäbchen und Zapfen im menschlichen Auge.

**Lösung:**
Drei wesentliche Unterschiede zwischen Stäbchen und Zapfen sind:

* [cite_start]**Lichtempfindlichkeit:** Stäbchen sind sehr lichtempfindlich und für das Sehen bei geringer Helligkeit (skotopisches Sehen) zuständig[cite: 1084]. [cite_start]Zapfen sind weniger lichtempfindlich und werden für das Sehen bei Tageslicht (photopisches Sehen) verwendet[cite: 1089].
* [cite_start]**Farbensehen:** Stäbchen können keine Farben unterscheiden und liefern nur Helligkeitsinformationen über ein schmales Spektrum[cite: 1086]. [cite_start]Zapfen gibt es in drei verschiedenen Typen, die auf unterschiedliche Wellenlängenbereiche spezialisiert sind und so das Farbensehen ermöglichen[cite: 1092].
* [cite_start]**Ortsverteilung auf der Retina:** Zapfen sind hauptsächlich im Zentrum des schärfsten Sehens, der Fovea, konzentriert[cite: 1202, 1212]. [cite_start]Stäbchen befinden sich vor allem in der Peripherie der Netzhaut[cite: 1210].

---

**Frage 5 (Berechnung)**

Berechnen Sie nach dem Hick'schen Gesetz die benötigte Zeit, um aus einem Menü mit 5 gleichwahrscheinlichen Optionen eine Auswahl zu treffen. Verwenden Sie die in der Vorlesung angegebenen Konstanten.

**Lösung:**
Die Formel nach Hick'schem Gesetz für mehrere Alternativen lautet:
[cite_start]$T = a + b \cdot \sum_{i} (p_i \cdot \text{ld}(\frac{1}{p_i} + 1))$ [cite: 2166]

Bei N gleichwahrscheinlichen Optionen ist die Wahrscheinlichkeit für jede Option $p_i = \frac{1}{N}$. Die Formel vereinfacht sich (analog zur Musterklausur) zu:
$T = a + b \cdot N \cdot (\frac{1}{N} \cdot \text{ld}(N + 1)) = a + b \cdot \text{ld}(N + 1)$

Gegebene Werte:
* Anzahl der Optionen $N = 5$
* [cite_start]Konstante $a = 50$ ms [cite: 2167]
* [cite_start]Konstante $b = 150$ ms [cite: 2167]

Berechnung:
1.  Term berechnen: $N + 1 = 5 + 1 = 6$
2.  Logarithmus dualis berechnen: $\text{ld}(6) = \log_2(6) \approx 2.585$
3.  In die Formel einsetzen: $T = 50 \text{ ms} + 150 \text{ ms} \cdot 2.585$
4.  Ausrechnen: $T \approx 50 + 387.75 = 437.75$ ms

Es dauert ungefähr **438 ms**, um die Auswahl zu treffen.

---
### Teil 2: Bildverarbeitung

**Frage 6 (Wissensfrage)**

Nennen Sie die 4 wesentlichen Schritte des Canny-Algorithmus zur Kantendetektion.

**Lösung:**
[cite_start]Die vier wesentlichen Schritte des Canny-Algorithmus sind[cite: 2504]:

1.  [cite_start]**Gaußsche Tiefpass-Filterung:** Zur Rauschunterdrückung im Vorfeld[cite: 2504].
2.  [cite_start]**Bestimmung der Gradientenstärke und -richtung:** Meist durch Sobel-Filter, um die partiellen Ableitungen zu ermitteln[cite: 2508, 2509].
3.  [cite_start]**Non-Maximum Suppression:** Unterdrückung von Pixeln, die nicht das lokale Maximum in Gradientenrichtung darstellen, um Kanten auf eine Breite von 1 Pixel zu verdünnen (Edge Thinning)[cite: 2510].
4.  [cite_start]**Hysterese (Zwei Schwellwerte):** Verwendung einer oberen und unteren Schwelle, um starke Kanten sicher zu finden und schwache Kanten nur dann zu berücksichtigen, wenn sie mit starken Kanten verbunden sind[cite: 2510].

---

**Frage 7 (Wissensfrage)**

Was ist der Zweck der "Rectification" in der Stereobildverarbeitung und wie wird sie erreicht?

**Lösung:**
* **Zweck:** Die Rectification dient der Vereinfachung der Korrespondenzsuche zwischen den beiden Stereobildern. [cite_start]Ziel ist es, die epipolaren Linien in beiden Bildern horizontal auszurichten[cite: 2561]. Dadurch muss ein zu einem Pixel im linken Bild korrespondierender Pixel im rechten Bild nur noch entlang derselben Bildzeile gesucht werden, was die Suche von einem 2D-Problem auf ein 1D-Problem reduziert.
* [cite_start]**Umsetzung:** Dies wird durch eine geometrische Transformation (eine projektive Transformation) der beiden Bilder erreicht, sodass die Epipole im Unendlichen liegen und die epipolaren Linien parallel und horizontal verlaufen[cite: 2561].

---

**Frage 8 (Wissensfrage / Erklärung)**

Erklären Sie den fundamentalen Unterschied zwischen einem Median-Filter und einem Mittelwert-Filter. Welcher Filter eignet sich besser zur Entfernung von „Salt-and-Pepper“-Rauschen und warum?

**Lösung:**

* **Fundamentaler Unterschied:**
    * Der **Mittelwert-Filter** ist ein linearer Filter. Er berechnet für jedes Pixel einen neuen Wert, indem er die Grauwerte aller Pixel in einer definierten Nachbarschaft arithmetisch mittelt. [cite_start]Dies führt zu einer Glättung des Bildes, bei der aber auch Kanten verschliffen werden[cite: 2382, 2383].
    * Der **Median-Filter** ist ein nicht-linearer Rangordnung-Filter. Er ersetzt den Wert eines Pixels durch den Median der Grauwerte in seiner Nachbarschaft. [cite_start]Dazu werden alle Grauwerte der Nachbarschaft sortiert und der mittlere Wert ausgewählt[cite: 2363, 2365].

* **Eignung für "Salt-and-Pepper"-Rauschen:**
    Der **Median-Filter** eignet sich deutlich besser.
    * [cite_start]**Begründung:** "Salt-and-Pepper"-Rauschen (auch Impulsrauschen [cite: 2343]) äußert sich durch einzelne, extrem helle (255) oder dunkle (0) Pixel. Diese extremen Werte sind in der sortierten Liste der Nachbarschaftswerte fast immer an den Rändern und werden daher bei der Auswahl des Medians (des mittleren Wertes) ignoriert. Ein Mittelwert-Filter würde diese Extremwerte in seine Berechnung einbeziehen und den Fehler lediglich auf die Nachbarschaft "verschmieren". [cite_start]Der Median-Filter erhält Kanten besser, da der Medianwert ein tatsächlich im Bild vorhandener Wert aus der Nachbarschaft ist[cite: 2365].

---

**Frage 9 (Wissensfrage)**

Was repräsentiert der Wert im Zentrum des Amplitudenspektrums (bei Frequenz u=0, v=0) nach einer 2D-Fouriertransformation? Wie äußern sich stark vertikale Strukturen eines Bildes im Amplitudenspektrum?

**Lösung:**

* [cite_start]**Zentrum F(0,0):** Der Wert im Zentrum des Frequenzspektrums, F(0,0), repräsentiert den **Gleichanteil (DC-Anteil)** des Bildes[cite: 2446]. [cite_start]Er entspricht der Summe aller Pixelintensitäten und damit der durchschnittlichen Helligkeit des Bildes[cite: 2434].
* **Vertikale Strukturen:** Stark ausgeprägte vertikale Strukturen im Bild (z.B. ein Gitter aus senkrechten Strichen) bedeuten hohe Ortsfrequenzen in horizontaler Richtung. [cite_start]Im Amplitudenspektrum äußert sich dies durch hohe Amplitudenwerte entlang der **horizontalen Frequenzachse (u-Achse)**, weg vom Zentrum[cite: 2448, 2454].

---
### Teil 3: Computergrafik

**Frage 10 (Wissensfrage)**

Aus welchen 3 Komponenten setzt sich das lokale Beleuchtungsmodell nach Phong zusammen? Beschreiben Sie kurz die jeweilige Wirkung.

**Lösung:**
[cite_start]Das lokale Beleuchtungsmodell nach Phong setzt sich aus den folgenden drei Komponenten zusammen[cite: 2759]:

1.  [cite_start]**Ambiente Komponente:** Simuliert eine allgemeine Grundhelligkeit der Szene, die durch indirekte, vielfach gestreute Beleuchtung entsteht[cite: 2758]. Sie ist unabhängig von der Position der Lichtquelle und dem Blickwinkel und sorgt dafür, dass auch nicht direkt beleuchtete Flächen nicht komplett schwarz sind.
2.  [cite_start]**Diffuse Komponente:** Repräsentiert die gerichtete, aber gleichmäßig in alle Richtungen gestreute Reflexion des Lichts von einer matten Oberfläche (Lambertsche Streuung)[cite: 2758]. Ihre Intensität hängt vom Winkel zwischen der Lichtquelle und der Oberflächennormalen ab, ist aber vom Betrachterstandpunkt unabhängig.
3.  [cite_start]**Spekulare Komponente:** Modelliert die spiegelnde Reflexion (Glanzlichter) von glatten, glänzenden Oberflächen[cite: 2758]. Ihre Intensität ist stark vom Blickwinkel des Betrachters abhängig und am größten, wenn der Reflexionswinkel dem Einfallswinkel des Lichts entspricht.

---

**Frage 11 (Berechnung / Anwendung)**

Geben Sie die resultierende Transformationsmatrix $M$ in homogenen Koordinaten an, die ein 3D-Objekt zuerst um 90° um die Z-Achse rotiert und anschließend um den Vektor $T = (5, 2, 0)$ verschiebt.

**Lösung:**
Die Transformationen müssen in umgekehrter Reihenfolge der Anwendung multipliziert werden: $M = \text{Translation} \cdot \text{Rotation}$.

1.  **Rotationsmatrix $R_z(90°)$:**
    [cite_start]Für eine Rotation um die Z-Achse gilt[cite: 2686]:
    $R_z(\alpha) = \begin{pmatrix} \cos\alpha & -\sin\alpha & 0 & 0 \\ \sin\alpha & \cos\alpha & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$
    Mit $\alpha = 90°$, $\cos(90°) = 0$ und $\sin(90°) = 1$:
    $R_z(90°) = \begin{pmatrix} 0 & -1 & 0 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$

2.  **Translationsmatrix $T(5, 2, 0)$:**
    [cite_start]Für eine Translation gilt[cite: 2685]:
    $T(t_x, t_y, t_z) = \begin{pmatrix} 1 & 0 & 0 & t_x \\ 0 & 1 & 0 & t_y \\ 0 & 0 & 1 & t_z \\ 0 & 0 & 0 & 1 \end{pmatrix}$
    $T(5, 2, 0) = \begin{pmatrix} 1 & 0 & 0 & 5 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$

3.  **Multiplikation $M = T \cdot R_z$:**
    $M = \begin{pmatrix} 1 & 0 & 0 & 5 \\ 0 & 1 & 0 & 2 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix} \cdot \begin{pmatrix} 0 & -1 & 0 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix} = \begin{pmatrix} 0 & -1 & 0 & 5 \\ 1 & 0 & 0 & 2 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$

Die resultierende Gesamt-Transformationsmatrix ist:
$M = \begin{pmatrix} 0 & -1 & 0 & 5 \\ 1 & 0 & 0 & 2 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$

---

**Frage 12 (Wissensfrage)**

Nennen Sie 3 wichtige Entwurfsprinzipien oder Eigenschaften von kubischen Bézier-Splines.

**Lösung:**
Drei wichtige Eigenschaften von Bézier-Splines sind:

1.  [cite_start]**Endpunkt-Interpolation:** Die Kurve verläuft exakt durch den ersten und den letzten Kontrollpunkt[cite: 2646].
2.  **Tangenten-Steuerung an den Endpunkten:** Die Tangente am Anfang der Kurve wird durch die Verbindungslinie der ersten beiden Kontrollpunkte definiert. [cite_start]Die Tangente am Ende wird durch die letzten beiden Kontrollpunkte definiert[cite: 2648, 2649].
3.  [cite_start]**Konvexe-Hülle-Eigenschaft:** Die gesamte Bézier-Kurve liegt immer vollständig innerhalb der konvexen Hülle, die von ihren Kontrollpunkten aufgespannt wird[cite: 2646].
