---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetPrintingPreview yapıcı. SheetPrintingPreview'in yapısı"
type: docs
url: /tr/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

SheetPrintingPreview yapısı

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | Çalışma Sayfası | Hangi elektronik tablonun yazdırılacağını belirtin. |
| seçenekler | ImageOrPrintOptions | ImageOrPrintOptions, çıktının bazı özelliklerini içerir |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Sayfa yazdırma önizlemesi oluşturun
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Değerlendirilen sayfa sayısını çıktı olarak ver
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


