---
title: "Klasse SlicerCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Slicers.SlicerCache Klasse. Stellt die Zusammenfassungsbeschreibung des Slicer-Cache dar"
type: docs
url: /de/net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

Stellt die zusammenfassende Beschreibung des Slicer‑Cache dar

```csharp
public class SlicerCache
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | (**Obsolete.**) Gibt an, wie Elemente ohne Daten des Slicers angezeigt werden. |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | Gibt an, ob der mit dem angegebenen Slicer-Cache verbundene Slicer auf einer Nicht-OLAP-Datenquelle basiert. |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | Gibt den Namen des Slicer-Cache zurück. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | Gibt eine SlicerCacheItem‑Sammlung zurück, die die Sammlung aller Elemente im Slicer-Cache enthält. Nur lesbar |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | Gibt den Namen dieses Slicer-Cache zurück. |

### Beispiele

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
            
            // Erstelle Beispieldaten
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
            
            // Pivot-Tabelle erstellen
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Füge Slicer hinzu und erhalte dessen Cache
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
            
            // Demonstriere die Verwendung von SlicerCache
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

### Siehe auch

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


