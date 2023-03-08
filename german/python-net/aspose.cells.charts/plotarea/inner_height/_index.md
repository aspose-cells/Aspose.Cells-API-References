---
title: inner_height Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 150
url: /de/python-net/aspose.cells.charts/plotarea/inner_height/
is_root: false
---
##  inner_height Eigentum

Ruft die Höhe des Diagrammbereichs in Einheiten von 1/4000 des Diagrammbereichs ab oder legt diese fest.

###  Bemerkungen

Der Zeichenbereich-Begrenzungsrahmen enthält den Zeichenbereich, Teilstriche (Teilstriche) und einen kleinen Rahmen um die Teilstriche.
Wenn der Wert nicht von MS Excel erstellt wird, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.


 Der**X**, **Y** , **Breite** Und**Höhe** von**Grundstücksfläche** stellt den Grundstücksbereich dar
 Begrenzungsrahmen, der den Plotbereich, Teilstriche (Teilstriche) und einen kleinen Rahmen um die Teilstriche enthält.
 Wenn Sie die tatsächliche Größe der Grundstücksfläche erfahren möchten, sollten Sie anrufen**InnerX** , **InnerY** , **Innere Breite** Und
**InnereHöhe** Eigenschaften.


Für Excel 2007 oder höher ist der Standardwert Null. Sie sollten get the value aufrufen, nachdem Sie Chart.Calculate() aufgerufen haben.
###  Definition:
```python
@property
def inner_height(self):
    ...
@inner_height.setter
def inner_height(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [PlotArea](/cells/de/python-net/aspose.cells.charts/plotarea)
