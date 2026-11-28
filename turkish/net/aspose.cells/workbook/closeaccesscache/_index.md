---
title: "Workbook.CloseAccessCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Veriye erişmek için önbellek kullanan oturumu kapatır"
type: docs
url: /tr/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Veriye erişmek için önbellekleri kullanan oturumu kapatır.

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
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ve koşullu biçimlendirme ekle
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Koşullu biçimlendirme ekle
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Koşullu biçimlendirme için erişim önbelleğini başlat
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Önbelleğe alınmış koşullu biçimlendirmeli hücrelere eriş
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Erişim önbelleğini kapatın
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


