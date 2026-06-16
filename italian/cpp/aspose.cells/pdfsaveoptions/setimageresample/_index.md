---
title: Aspose::Cells::PdfSaveOptions::SetImageResample method
linktitle: SetImageResample
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetImageResample method. Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled in C++.'
type: docs
weight: 1800
url: /it/cpp/aspose.cells/pdfsaveoptions/setimageresample/
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
//Il codice seguente imposta i PPI desiderati a 96 e la qualità JPEG a 80 per le immagini nel PDF di output.

//carica il file di origine con le immagini.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//imposta i PPI desiderati a 96 e la qualità JPEG a 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
