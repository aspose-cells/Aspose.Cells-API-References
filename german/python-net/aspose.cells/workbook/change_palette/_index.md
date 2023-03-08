---
title: change_palette Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells/workbook/change_palette/
is_root: false
---
##  change_palette(color, index) {#aspose.pydrawing.Color-int}
Ändert die Palette für das Arbeitsblatt im angegebenen Index.



```python
def change_palette(self, color, index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Farbstruktur.|
| index | int | Palettenindex, 0 - 55.|
###  Bemerkungen

Die Palette hat 56 Einträge, die jeweils durch einen RGB-Wert dargestellt werden.


Wenn Sie eine Farbe einstellen, die nicht in der Palette enthalten ist, wird sie nicht wirksam.


Wenn Sie also eine benutzerdefinierte Farbe festlegen möchten, ändern Sie bitte zuerst die Palette.


Das Folgende ist die Standardfarbpalette.

| Farbe| Rot| Grün| Blau|
| :- | :- | :- | :- |
| Schwarz| 0| 0| 0 |
| Weiss| 255| 255| 255 |
| Rot| 255| 0| 0 |
| Kalk| 0| 255| 0 |
| Blau| 0| 0| 255 |
| Gelb| 255| 255| 0 |
| Magenta| 255| 0| 255 |
| Cyan| 0| 255| 255 |
| Kastanienbraun| 128| 0| 0 |
| Grün| 0| 128| 0 |
| Marine| 0| 0| 128 |
| Olive| 128| 128| 0 |
| Lila| 128| 0| 128 |
| Blaugrün| 0| 128| 128 |
| Silber| 192| 192| 192 |
| Grau| 128| 128| 128 |
| Farbe17| 153| 153| 255 |
| Farbe18| 153| 51| 102 |
| Farbe19| 255| 255| 204 |
| Farbe20| 204| 255| 255 |
| Farbe21| 102| 0| 102 |
| Farbe22| 255| 128| 128 |
| Farbe23| 0| 102| 204 |
| Farbe24| 204| 204| 255 |
| Farbe25| 0| 0| 128 |
| Farbe26| 255| 0| 255 |
| Farbe27| 255| 255| 0 |
| Farbe28| 0| 255| 255 |
| Farbe29| 128| 0| 128 |
| Farbe30| 128| 0| 0 |
| Farbe31| 0| 128| 128 |
| Farbe32| 0| 0| 255 |
| Farbe33| 0| 204| 255 |
| Farbe34| 204| 255| 255 |
| Farbe35| 204| 255| 204 |
| Farbe36| 255| 255| 153 |
| Farbe37| 153| 204| 255 |
| Farbe38| 255| 153| 204 |
| Farbe39| 204| 153| 255 |
| Farbe40| 255| 204| 153 |
| Farbe41| 51| 102| 255 |
| Farbe42| 51| 204| 204 |
| Farbe43| 153| 204| 0 |
| Farbe44| 255| 204| 0 |
| Farbe45| 255| 153| 0 |
|Farbe46| 255| 102| 0 |
| Farbe47| 102| 102| 153 |
| Farbe48| 150| 150| 150 |
| Farbe49| 0| 51| 102 |
| Farbe50| 51| 153| 102 |
| Farbe51| 0| 51| 0 |
| Farbe52| 51| 51| 0 |
| Farbe53| 153| 51| 0 |
| Farbe54| 153| 51| 102 |
| Farbe55| 51| 51| 153 |
| Farbe56| 51| 51| 51 |


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
