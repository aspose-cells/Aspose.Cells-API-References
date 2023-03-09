---
title: metodo to_image
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
##  to_image(page_index, file_name) {#int-str}
Renderizza determinate pagine in un file.



```python
def to_image(self, page_index, file_name):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| page_index | int | indicare quale pagina deve essere convertita|
| file_name | str | nome file dell'immagine di output|

###  Esempi

Il codice seguente emette la prima pagina del primo foglio in un'immagine png.

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.image_type = ImageType.PNG
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output the first page of the sheet to image.
sr.to_image(0, "output.png")

```


##  to_image(page_index, stream) {#int-io.RawIOBase}
Eseguire il rendering di determinate pagine in un flusso.



```python
def to_image(self, page_index, stream):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| page_index | int | indicare quale pagina deve essere convertita|
| stream | io.RawIOBase | il flusso dell'immagine di output|



###  Guarda anche
* modulo [aspose.cells.rendering](../../)
* classe [SheetRender](/cells/it/python-net/aspose.cells.rendering/sheetrender)
