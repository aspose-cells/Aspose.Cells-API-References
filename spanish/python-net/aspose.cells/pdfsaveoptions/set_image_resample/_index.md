---
title: set_image_resample método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---
##  set_image_resample(desired_ppi, jpeg_quality) {#int-int}
 Establece los PPI (píxeles por pulgada) deseados de las imágenes de remuestreo y la calidad jpeg.
 Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada,
y las imágenes que superen los PPI (píxeles por pulgada) especificados se volverán a muestrear.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| desired_ppi | int | Píxeles por pulgada deseados 220 alta calidad 150 calidad de pantalla 96 calidad de correo electrónico|
| jpeg_quality | int | 0 - 100% JPEG calidad.|

###  Ejemplos

El siguiente código establece el PPI deseado en 96 y la calidad jpeg en 80 para las imágenes en el pdf de salida.

```python
from aspose.cells import PdfSaveOptions, Workbook

# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [PdfSaveOptions](/cells/es/python-net/aspose.cells/pdfsaveoptions)
