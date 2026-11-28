---
title: "Worksheet.StartAccessCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu başlatır"
type: docs
url: /tr/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu başlatır.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | AccessCacheOptions | veri erişim seçenekleri |

### Açıklamalar

Verilere erişimi tamamladıktan sonra, [`CloseAccessCache`](../closeaccesscache/) aynı seçeneklerle çağrılmalı, tüm önbellekleri temizlemek ve normal erişim moduna geri dönmek için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Varsayılan stili ayarla
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Bazı verileri doldurun
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Daha iyi performans için erişim önbelleğini başlat
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Stilleri doğrula
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Tamamlandığında önbelleği kapat
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


