---
title: set_outline_borders Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells/unionrange/set_outline_borders/
is_root: false
---
##  set_outline_borders(border_styles, border_colors) {#list-aspose.pydrawing.Color[]}
Legt Linienränder um einen Bereich von Zellen fest.



```python
def set_outline_borders(self, border_styles, border_colors):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| border_styles | list | Rahmenstile.|
| border_colors | aspose.pydrawing.Color[] | Grenzfarben.|
###  Bemerkungen

Sowohl die Länge von borderStyles als auch von borderStyles muss 4 sein.
Die Reihenfolge von borderStyles und borderStyles muss oben, unten, links, rechts sein

##  set_outline_borders(border_style, border_color) {#CellBorderType-aspose.pydrawing.Color}
Legt die Umrissrahmen um einen Bereich von Zellen mit demselben Rahmenstil und derselben Farbe fest.



```python
def set_outline_borders(self, border_style, border_color):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| border_style | [CellBorderType](/cells/de/python-net/aspose.cells/cellbordertype) | Grenzstil.|
| border_color | aspose.pydrawing.Color | Randfarbe.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [UnionRange](/cells/de/python-net/aspose.cells/unionrange)
