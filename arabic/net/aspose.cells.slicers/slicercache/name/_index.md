---
title: "SlicerCache.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SlicerCache. تُرجع اسم ذاكرة التخزين المؤقت للمقسم"
type: docs
url: /ar/net/aspose.cells.slicers/slicercache/name/
---
## SlicerCache.Name property

يرجع اسم ذاكرة التخزين المؤقت لأداة التقطيع.

```csharp
public string Name { get; }
```

### أمثلة

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

### انظر أيضًا

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


