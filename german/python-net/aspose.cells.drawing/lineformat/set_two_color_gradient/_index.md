---
title: set_two_color_gradient Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest.
Gilt nur für Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Eine Verlaufsfarbe.|
| color2 | aspose.pydrawing.Color | Zwei Verlaufsfarben.|
| style | [GradientStyleType](/cells/de/python-net/aspose.cells.drawing/gradientstyletype) | Verlaufsschattierungsstil.|
| variant | int |Die Verlaufsvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte „Verlauf“ im Dialogfeld „Fülleffekte“. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest.
Gilt nur für Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Eine Verlaufsfarbe.|
| transparency1 | float | Der Transparenzgrad der Farbe1 als Wert von 0,0 (deckend) bis 1,0 (klar).|
| color2 | aspose.pydrawing.Color | Zwei Verlaufsfarben.|
| transparency2 | float | Der Transparenzgrad der Farbe2 als Wert von 0,0 (deckend) bis 1,0 (klar).|
| style | [GradientStyleType](/cells/de/python-net/aspose.cells.drawing/gradientstyletype) | Verlaufsschattierungsstil.|
| variant | int |Die Verlaufsvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte „Verlauf“ im Dialogfeld „Fülleffekte“. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein.|



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [LineFormat](/cells/de/python-net/aspose.cells.drawing/lineformat)
