---
title: "PdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions yöntemi. Yeniden örneklenen görüntülerin istenen PPI (inç başına piksel) ve jpeg kalitesini ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI inç başına piksel değerinden büyük olan görüntüler yeniden örneklenir"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

İstenen PPI (inç başına piksel) değerini yeniden örnekleme görüntüleri ve jpeg kalitesi için ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI (inç başına piksel) değerinden büyük olan görüntüler yeniden örneklenir.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredPPI | Int32 | İnç başına istenen piksel. 220 yüksek kalite. 150 ekran kalitesi. 96 e-posta kalitesi. |
| jpegQuality | Int32 | 0 - %100 JPEG kalitesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("Book1.xlsx");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SetImageResample(96, 80);
            
            wb.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


