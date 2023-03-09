---
title: get_picture metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 120
url: /sv/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Hämtar objektet [Picture](/cells/sv/python-net/aspose.cells.drawing/picture) i sidhuvudet/sidfoten.


###  Returnerar

Returnerar [Picture](/cells/sv/python-net/aspose.cells.drawing/picture) objekt.
Returnerar null om det inte finns någon bild.


```python
def get_picture(self, is_header, section):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| is_header | bool | Indikerar om det finns i sidhuvudet eller sidfoten.|
| section | int | 0: Vänster sektion, 1: Mittsektion, 2: Höger sektion.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Hämtar objektet [Picture](/cells/sv/python-net/aspose.cells.drawing/picture) i sidhuvudet/sidfoten.


###  Returnerar

Returnerar [Picture](/cells/sv/python-net/aspose.cells.drawing/picture) objekt.


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| is_first | bool | Indikerar om bilden av första sidans sidhuvud/sidfot hämtas.|
| is_even | bool | Indikerar om bilden av sidhuvud/sidfot på jämna sidor.|
| is_header | bool | Indikerar om bilden av sidhuvud/sidfot hämtas.|
| section | int | 0: Vänster sektion, 1: Mittsektion, 2: Höger sektion.|



###  Se även
* modul [aspose.cells](../../)
* klass [PageSetup](/cells/sv/python-net/aspose.cells/pagesetup)
* klass [Picture](/cells/sv/python-net/aspose.cells.drawing/picture)
