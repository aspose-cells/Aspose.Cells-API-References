---
title: "Top10Filter.Items"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10Filter-egenskap. Hämtar och anger övre eller nedre värde att använda som filterkriterium"
type: docs
url: /sv/net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

Hämtar och anger över- eller undervärde att använda som filterkriterium.

```csharp
public int Items { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyItemsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grapes");
            worksheet.Cells["A6"].PutValue("Mango");
            
            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Tillämpa top 10-filter
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Hämta filtret och demonstrera Items-egenskapen
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            int itemsCount = filter.GetTop10Value().Items;
            
            Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
        }
    }
}
```

### Se även

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


