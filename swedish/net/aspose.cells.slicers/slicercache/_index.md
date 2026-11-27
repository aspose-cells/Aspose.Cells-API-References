---
title: "Klass SlicerCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Slicers.SlicerCache-klass. Representerar en sammanfattande beskrivning av skärmningscachen."
type: docs
url: /sv/net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

Representerar sammanfattande beskrivning av slicer-cache.

```csharp
public class SlicerCache
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | (**Obsolete.**) Indikerar hur man visar objekt utan data i skärmningskontrollen. |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | Indikerar om skärmningskontrollen som är associerad med den angivna skärmningscachen är baserad på en icke‑OLAP-datakälla. |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | Returnerar namnet på skärmningscachen. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | Returnerar en SlicerCacheItem‑samling som innehåller alla objekt i skärmningscachen. Endast läs. |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | Returnerar namnet på denna skärmningscache. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Skapa exempeldata
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";
            
            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;
            
            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;
            
            // Skapa pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Lägg till skärmningskontrollen och hämta dess cache.
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
            
            // Demonstrera användning av SlicerCache.
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Items:");
            foreach (SlicerCacheItem item in slicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            book.Save("out.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


