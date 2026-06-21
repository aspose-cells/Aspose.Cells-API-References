---
title: Aspose::Cells::PdfSaveOptions::SetImageResample method
linktitle: SetImageResample
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetImageResample method. Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled in C++.'
type: docs
weight: 1800
url: /de/cpp/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions::SetImageResample method


Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.

```cpp
void Aspose::Cells::PdfSaveOptions::SetImageResample(int32_t desiredPPI, int32_t jpegQuality)
```


| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | int32_t | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | int32_t | 0 - 100% JPEG quality. |


## Examples


```cpp
Aspose::Cells::Startup();
//Der folgende Code setzt die gewünschte PPI auf 96 und die JPEG‑Qualität auf 80 für Bilder im Ausgabe‑PDF.

//Laden Sie die Quelldatei mit Bildern.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//Setzen Sie die gewünschte PPI auf 96 und die JPEG‑Qualität auf 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
