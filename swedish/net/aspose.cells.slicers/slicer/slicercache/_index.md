---
title: "Slicer.SlicerCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Returnerar SlicerCache-objektet som är associerat med slicern. Endast läsning"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/slicercache/
---
## Slicer.SlicerCache property

Returnerar SlicerCache-objektet som är associerat med slicern. Endast läsning.

```csharp
public SlicerCache SlicerCache { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertySlicerCacheDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Skapa en tabell från dataområdet
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Lägg till en skivkontroll
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Demonstrera användning av SlicerCache.
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
            Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
            Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);

            // Spara arbetsboken
            workbook.Save("SlicerCacheDemo.xlsx");
        }
    }
}
```

### Se även

* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


