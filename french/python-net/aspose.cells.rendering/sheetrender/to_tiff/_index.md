---
title: to_tiff méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells.rendering/sheetrender/to_tiff/
is_root: false
---
##  to_tiff(stream) {#io.RawIOBase}
Rendre la feuille de calcul entière en tant qu'image Tiff à diffuser.



```python
def to_tiff(self, stream):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | le flux de l'image de sortie|


##  to_tiff(filename) {#str}
Rendre la feuille de calcul entière en tant qu'image Tiff dans un fichier.



```python
def to_tiff(self, filename):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| filename | str | le nom de fichier de l'image de sortie|

###  Exemple

Le code suivant sort toutes les pages de la première feuille en image Tiff.

```python
from aspose.cells import SaveFormat, Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.save_format = SaveFormat.TIFF
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output all the pages of the sheet to Tiff image.
sr.to_tiff("output.tiff")

```



###  Voir également
* module [aspose.cells.rendering](../../)
* classe [SheetRender](/cells/fr/python-net/aspose.cells.rendering/sheetrender)
