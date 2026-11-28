---
title: "CellWatch.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellWatch özelliği. Hücrenin satırını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Hücrenin satırını alır ve ayarlar.

```csharp
public int Row { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // B2 hücresine örnek veri ekle
            sheet.Cells["B2"].PutValue("Sample Data");

            // B2 için CellWatch ekle
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Row özelliğini göster
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Hücre referansını doğrula
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


