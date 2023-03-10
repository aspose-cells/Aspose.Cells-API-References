---
title: change_palette metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/workbook/change_palette/
is_root: false
---
##  change_palette(color, index) {#aspose.pydrawing.Color-int}
Ändrar paletten för kalkylarket i det angivna indexet.



```python
def change_palette(self, color, index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Färgstruktur.|
| index | int | Palettindex, 0 - 55.|
###  Anmärkningar

Paletten har 56 poster, var och en representerad av ett RGB-värde.


Om du ställer in en färg som inte finns i paletten kommer den inte att träda i kraft.


Så om du vill ställa in en anpassad färg, vänligen ändra paletten först.


Följande är standardfärgpaletten.

| Färg| Röd| Grön| Blå|
| :- | :- | :- | :- |
| Svart| 0| 0| 0 |
| Vit| 255| 255| 255 |
| Röd| 255| 0| 0 |
| Kalk| 0| 255| 0 |
| Blå| 0| 0| 255 |
| Gul| 255| 255| 0 |
| Magenta| 255| 0| 255 |
| Cyan| 0| 255| 255 |
| Rödbrun| 128| 0| 0 |
| Grön| 0| 128| 0 |
| Marin| 0| 0| 128 |
| Oliv| 128| 128| 0 |
| Lila| 128| 0| 128 |
| Kricka| 0| 128| 128 |
| Silver| 192| 192| 192 |
| grå| 128| 128| 128 |
| Färg17| 153| 153| 255 |
| Färg18| 153| 51| 102 |
| Färg19| 255| 255| 204 |
| Färg20| 204| 255| 255 |
| Färg 21| 102| 0| 102 |
| Färg22| 255| 128| 128 |
| Färg23| 0| 102| 204 |
| Färg24| 204| 204| 255 |
| Färg25| 0| 0| 128 |
| Färg26| 255| 0| 255 |
| Färg27| 255| 255| 0 |
| Färg28| 0| 255| 255 |
| Färg29| 128| 0| 128 |
| Färg30| 128| 0| 0 |
| Färg31| 0| 128| 128 |
| Färg32| 0| 0| 255 |
| Färg33| 0| 204| 255 |
| Färg34| 204| 255| 255 |
| Färg35| 204| 255| 204 |
| Färg36| 255| 255| 153 |
| Färg37| 153| 204| 255 |
| Färg38| 255| 153| 204 |
| Färg39| 204| 153| 255 |
| Färg40| 255| 204| 153 |
| Färg41| 51| 102| 255 |
| Färg42| 51| 204| 204 |
| Färg43| 153| 204| 0 |
| Färg44| 255| 204| 0 |
| Färg45| 255| 153| 0 |
| Färg46| 255| 102| 0 |
| Färg47| 102| 102| 153 |
| Färg48| 150| 150| 150 |
| Färg49| 0| 51| 102 |
| Färg50| 51| 153| 102 |
| Färg51| 0| 51| 0 |
| Färg52| 51| 51| 0 |
| Färg53| 153| 51| 0 |
|Färg54| 153| 51| 102 |
| Färg55| 51| 51| 153 |
| Färg56| 51| 51| 51 |


###  Se även

* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
