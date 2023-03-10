---
title: set_image_resample metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---
##  set_image_resample(desired_ppi, jpeg_quality) {#int-int}
 Ställer in önskad PPI (pixlar per tum) för omsamplingsbilder och jpeg-kvalitet.
 Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen,
och bilder som är större än den angivna PPI (pixlar per tum) omsamplas.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| desired_ppi | int | Önskade pixlar per tum. 220 hög kvalitet. 150 skärmkvalitet. 96 e-postkvalitet.|
| jpeg_quality | int | 0 - 100 % JPEG kvalitet.|

###  Exempel

Följande kod anger önskad PPI som 96 och jpeg-kvalitet som 80 för bilder i utdata-pdf.

```python
from aspose.cells import PdfSaveOptions, Workbook

# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)

```



###  Se även
* modul [aspose.cells](../../)
* klass [PdfSaveOptions](/cells/sv/python-net/aspose.cells/pdfsaveoptions)
