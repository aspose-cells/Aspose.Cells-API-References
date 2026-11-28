---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Otomatik sayfa sonlarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

Otomatik sayfa sonlarını alır.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | ImageOrPrintOptions | Yazdırma seçenekleri |

### Dönüş Değeri

Otomatik sayfa sonları alanları.

### Açıklamalar

Her hücre alanı bir kağıdı temsil eder.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfa sonları oluşturmak için örnek veri ekleyin
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // Yazdırma alanını ve sayfa ayarını belirleyin
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // ImageOrPrintOptions ile sayfa sonlarını alın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // İlk sayfa sonu bilgisini çıktı olarak ver
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


