---
title: "Worksheet.CloseAccessCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu kapatır"
type: docs
url: /tr/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Bu çalışma sayfasındaki verilere erişmek için önbellek kullanan oturumu kapatır.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | AccessCacheOptions | veri erişim seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Hücreleri örnek veriyle doldurun
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Koşullu biçimlendirme ekle
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Koşullu biçimlendirme için erişim önbelleğini etkinleştirin
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Önbellekli erişimle işlemler gerçekleştirin
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Erişim önbelleğini kapatın
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Ayrıca Bakınız

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


