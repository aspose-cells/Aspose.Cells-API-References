---
title: "Worksheet.CellWatches"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasındaki izleme penceresinde izlenen hücrelerin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Bu çalışma sayfasındaki 'watch window' içinde izlenen hücre koleksiyonunu alır.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // B2 hücresine örnek veri ekle
            sheet.Cells["B2"].PutValue("Sample Data");

            // B2 için Hücre İzleme ekle
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // İzleme bilgilerini göster
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Çalışma kitabını kaydedin
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


