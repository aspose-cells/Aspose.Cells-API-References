---
title: set_one_color_gradient Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/
is_root: false
---
##  set_one_color_gradient(color, degree, style, variant) {#aspose.pydrawing.Color-float-GradientStyleType-int}
Legt die angegebene Füllung auf einen einfarbigen Farbverlauf fest.
Gilt nur für Excel 2007.



```python
def set_one_color_gradient(self, color, degree, style, variant):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Eine Verlaufsfarbe.|
| degree | float | Der Steigungsgrad. Kann ein Wert von 0,0 (dunkel) bis 1,0 (hell) sein.|
| style | [GradientStyleType](/cells/de/python-net/aspose.cells.drawing/gradientstyletype) | Verlaufsschattierungsstil.|
| variant | int |Die Verlaufsvariante. Kann ein Wert zwischen 1 und 4 sein, der einer der vier Varianten auf der Registerkarte „Verlauf“ im Dialogfeld „Fülleffekte“ entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein.|



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [FillFormat](/cells/de/python-net/aspose.cells.drawing/fillformat)
