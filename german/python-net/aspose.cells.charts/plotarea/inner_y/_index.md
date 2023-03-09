---
title: inner_y Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells.charts/plotarea/inner_y/
is_root: false
---
##  inner_y Eigentum

Ruft die x-Koordinate der oberen oberen Ecke des Diagrammbereichs in Einheiten von 1/4000 des Diagrammbereichs ab oder ruft diese ab.

###  Bemerkungen

Der Plotbereich-Begrenzungsrahmen umfasst den Plotbereich, Teilstriche (Teilstrichetiketten) und einen kleinen Rahmen um die Teilstriche.
 Wenn der Wert nicht von MS Excel erstellt wird, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.


 Der**X**, **Y** , **Breite** Und**Höhe** von**Grundstücksfläche** stellt den Grundstücksbereich dar
 Ein Begrenzungsrahmen, der den Plotbereich, Teilstriche (Teilstrichbeschriftungen) und einen kleinen Rahmen um die Teilstriche enthält.
 Wenn Sie die tatsächliche Größe der Grundstücksfläche erfahren möchten, sollten Sie anrufen**Inneres X** , **Inneres Y** , **Innere Breite** Und
**Innere Höhe** Eigenschaften.


Für Excel 2007 oder höher ist der Standardwert Null.
###  Definition:
```python
@property
def inner_y(self):
    ...
@inner_y.setter
def inner_y(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [PlotArea](/cells/de/python-net/aspose.cells.charts/plotarea)
