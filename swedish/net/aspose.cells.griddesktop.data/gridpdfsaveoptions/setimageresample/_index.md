---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridPdfSaveOptions-metod. Ställer in önskad PPI (pixlar per tum) för omprovade bilder och JPEG-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen och bilder som är större än den angivna PPI-pixlar per tum kommer att omprovas."
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Anger önskad PPI (pixlar per tum) för omprovningsbilder och JPEG-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att omprovas.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredPPI | Int32 | Önskade pixlar per tum. 220 hög kvalitet. 150 skärmkvalitet. 96 e-postkvalitet. |
| jpegQuality | Int32 | 0 - 100 % JPEG-kvalitet. |

### Exempel

Följande kod ställer in önskad PPI till 96 och JPEG-kvalitet till 80 för bilder i den genererade PDF-filen.

```csharp
//läs in källfilen med bilder.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//ställ in önskad PPI till 96 och JPEG-kvalitet till 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Se även

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


