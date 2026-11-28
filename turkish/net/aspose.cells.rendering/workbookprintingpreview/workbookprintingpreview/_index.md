---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookPrintingPreview yapıcı. WorkbookPrintingPreview'in oluşturulması"
type: docs
url: /tr/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

WorkbookPrintingPreview yapısı

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çalışma kitabı | Çalışma Kitabı | Yazdırılacak çalışma kitabını belirtin. |
| seçenekler | ImageOrPrintOptions | ImageOrPrintOptions, çıktının bazı özelliklerini içerir |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Yazdırma seçeneklerini ayarlayın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Çalışma kitabı ve seçeneklerle yazdırma önizlemesi oluşturun
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Sayfa sayısını göster
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


