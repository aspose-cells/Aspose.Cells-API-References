---
title: metodo set_image_resample
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---
##  set_image_resample(desired_ppi, jpeg_quality) {#int-int}
 Imposta il PPI desiderato (pixel per pollice) delle immagini di ricampionamento e la qualità jpeg.
 Tutte le immagini verranno convertite in JPEG con l'impostazione di qualità specificata,
e le immagini più grandi del PPI (pixel per pollice) specificato verranno ricampionate.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| desired_ppi | int | Pixel per pollice desiderati. 220 alta qualità. 150 qualità schermo. 96 qualità e-mail.|
| jpeg_quality | int | 0 - 100% JPEG qualità.|

###  Esempi

Il codice seguente imposta il PPI desiderato su 96 e la qualità jpeg su 80 per le immagini nel pdf di output.

```python
from aspose.cells import PdfSaveOptions, Workbook

# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/it/python-net/aspose.cells/pdfsaveoptions)
