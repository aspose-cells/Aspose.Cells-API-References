---
title: "Enum AdjustFontSizeForRowType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Hangi tür satırların ayarlanması gerektiğini temsil eder"
type: docs
url: /tr/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Hangi tür satırların ayarlanması gerektiğini temsil eder.

```csharp
public enum AdjustFontSizeForRowType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Ayarlama yok. |
| EmptyRows | `1` | Satır boşsa, satır yüksekliğine sığacak şekilde yazı tipi boyutunu değiştir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekleyin.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // AdjustFontSizeForRowType ayarıyla PptxSaveOptions bir örnek oluşturun
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Çalışma kitabını PPTX dosyası olarak kaydedin
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


