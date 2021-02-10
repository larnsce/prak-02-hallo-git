Praktikum 01 - Hallo R
================
Füge deinen Namen hier hinzu
Füge das Datum hier hinzu

## Lade Packages und Daten

``` r
library(tidyverse) 
library(datasauRus)
```

## Übungen

### Übung 1

Entferne diesen Text und füge deine Antwort für Übung 1 hier ein.

``` r
?datasaurus_dozen
```

### Übung 2

Die Antworten für diese Übung sind unter bereits für dich angegeben. Du
solltest aber den Text überarbeiten und nur das für dich relevante
eingeben.

Zuerst plotten wir den Dino Datensatz

``` r
dino_data <- datasaurus_dozen %>%
  filter(dataset == "dino")

ggplot(data = dino_data, mapping = aes(x = x, y = y)) +
  geom_point()
```

![](prak-01_files/figure-gfm/plot-dino-1.png)<!-- -->

Und als nächstes berechne die Korrelation zwischen “x” und “y” in diesem
Datensatz:

``` r
dino_data %>%
  summarize(r = cor(x, y))
```

    ## # A tibble: 1 x 1
    ##         r
    ##     <dbl>
    ## 1 -0.0645

### Übung 3

Füge den Code und die Beschreibungen nach Bedarf hinzu. Beachte, dass
die R-Chunks mit `plot-star` und `cor-star` beschriftet sind, um Platz
für den Code zum Plotten und Berechnen des Korrelationskoeffizienten zu
schaffen.

Bereinige zum Schluss den Text, indem du diese Anweisungen entfernst.

Blah blah blah…

Ich bin irgendein Text, du solltest mich durch einen sinnvolleren Text
ersetzen…

### Übung 4

Füge den Code und die Beschreibung nach Bedarf hinzu. Beachte, dass zwei
R-Blöcke gegeben sind, die aber nicht beschriftet sind. Verwende die
Konvention von oben, um sie entsprechend zu benennen.

### Übung 5

Füge den Code und die Beschreibung nach Bedarf hinzu. R Chunks kannst du
folgendermassen hinzufügen:

-   Benutze den Button Chunk oben, grünes C+, und klicke auf R
-   Nutze das Tastatur-Kürzel: `Cmd + Option + I` (Mac) oder
    `Ctrl + Alt + I` (Windows/Linux)
-   Mach dir die Mühe und schreib die Backticks, die geschweiften
    Klammern und den Buchstaben `r`
