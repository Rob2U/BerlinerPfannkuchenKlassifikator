# Berliner vs. Pfannkuchen -- Übungsblatt 7

## Aufgabe 1
1. Für dieses Aufgabenblatt wird versucht herauszufinden, ob es möglich ist den Berlinern unter die Arme zu greifen, wenn es darum geht den richtigen Begriff für Pfannkuchen und Berliner herauszufinden bzw. diese richtig zu zuordnen. Dafür wurde mit dem [hier](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator/blob/main/src/scraping.ipynb) zu findenden Notebook Bilder der jeweiligen Speisen durch Scraping von Google gesammelt. Diese Bilder wurden danach auf eine Größe von 112x112x3 (RGB) gebracht und gespeichert. Um die Daten nocheinmal zu Filtern wurden per Hand noch Säuberungen (falsche Bilder gelöscht) vorgenommen.
2. Das Ziel ist, wie bereits in 1. angesprochen wurde anhand eines Bilder zu klassifizieren, ob es sich um einen Pfannkuchen oder Berliner handelt.
3. ---
4. [hier](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator) zu finden (gesammter Code). Es wurde ein Split in Train-, Validation- und Test-Mengen. Insgesamt gibt es 2*297 Bilder. 70% werden davon zum Trainieren, 20% zum Validieren und 10% zum Testen benutzt.


## Aufgabe 2
1. [cnn.ipynb](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator/blob/main/src/scraping.ipynb) bzw. [tl_resenet.ipynb](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator/blob/main/src/tl_resenet.ipynb)
2. Das selbst erstellte und vollständig selbst trainierte Convolutional Neural Network erreicht bereits nach kurzem Training eine Genauigkeit von rund 85-90%. Gleichzeitg erreicht das zweite Modell, ein um eine Dropout- und eine FullyConnected-Schicht erweitertes ResNet18, eine Genauigkeit von ungefähr 80-85% auf den Testdaten.
3. (siehe [cnn.ipynb](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator/blob/main/src/scraping.ipynb) bzw. [tl_resenet.ipynb](https://github.com/Rob2U/BerlinerPfannkuchenKlassifikator/blob/main/src/tl_resenet.ipynb) enthält auch noch Konfusion-Matrix)