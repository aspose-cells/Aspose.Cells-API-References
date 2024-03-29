---
title: SetImageResample
second_title: Aspose.Cells för .NET API-referens
description: Ställer in önskad PPI pixlar per tum för omsamplingsbilder och jpeg-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen och bilder som är större än den angivna PPI pixlar per tum kommer att samplas om.
type: docs
weight: 320
url: /sv/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Ställer in önskad PPI (pixlar per tum) för omsamplingsbilder och jpeg-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att samplas om.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredPPI | Int32 | Önskade pixlar per tum. 220 hög kvalitet. 150 skärmkvalitet. 96 e-postkvalitet. |
| jpegQuality | Int32 | 0 - 100 % JPEG-kvalitet. |

### Exempel

Följande kod anger önskad PPI som 96 och jpeg-kvalitet som 80 för bilder i utdata pdf.

```csharp
//ladda in källfilen med bilder.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//ställ in önskad PPI som 96 och jpeg-kvalitet som 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Se även

* class [PdfSaveOptions](../../pdfsaveoptions)
* namnutrymme [Aspose.Cells](../../pdfsaveoptions)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
