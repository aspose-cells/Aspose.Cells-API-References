---
title: "SlicerCache.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SlicerCache-Eigenschaft. Gibt den Namen des Slicer-Caches zurück"
type: docs
url: /de/net/aspose.cells.slicers/slicercache/name/
---
## SlicerCache.Name property

Gibt den Namen des Slicer-Cache zurück.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Banana";
            sheet.Cells["A4"].Value = "Cherry";
            
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "E1");
            Slicer slicer = sheet.Slicers[slicerIndex];
            Console.WriteLine("Slicer Cache Name: " + slicer.SlicerCache.Name);
        }
    }
}
```

### Siehe auch

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


