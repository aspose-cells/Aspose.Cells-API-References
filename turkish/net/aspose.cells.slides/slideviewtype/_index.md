---
title: "Enum SlideViewType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Slides.SlideViewType enum. Slaytlara dışa aktarırken türü temsil eder"
type: docs
url: /tr/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Slaytlara dışa aktarırken türü temsil eder.

```csharp
public enum SlideViewType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| View | `0` | MS Excel'de görünüm olarak dışa aktarılıyor. |
| Print | `1` | Yazdırma olarak dışa aktarılıyor. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // SlideViewType ile PPTX kaydetme seçeneklerini yapılandırın
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // PPTX olarak kaydet
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


