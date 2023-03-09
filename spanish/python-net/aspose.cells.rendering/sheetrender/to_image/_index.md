---
title: to_image método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
##  to_image(page_index, file_name) {#int-str}
Renderizar cierta página a un archivo.



```python
def to_image(self, page_index, file_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| page_index | int | indicar qué página se va a convertir|
| file_name | str | nombre de archivo de la imagen de salida|

###  Ejemplo

El siguiente código genera la primera página de la primera hoja en una imagen png.

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
Renderizar cierta página a una secuencia.



```python
def to_image(self, page_index, stream):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| page_index | int | indicar qué página se va a convertir|
| stream | io.RawIOBase | el flujo de la imagen de salida|



###  Ver también
* módulo [aspose.cells.rendering](../../)
* clase [SheetRender](/cells/es/python-net/aspose.cells.rendering/sheetrender)
