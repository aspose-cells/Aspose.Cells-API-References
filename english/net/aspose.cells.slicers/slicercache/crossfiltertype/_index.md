---
title: SlicerCache.CrossFilterType
second_title: Aspose.Cells for .NET API Reference
description: SlicerCache property. Indicates how to show items with no data of slicer
type: docs
url: /net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Indicates how to show items with no data of slicer.

```csharp
[Obsolete("Use Slicer.ShowTypeOfItemsWithNoData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use [`ShowTypeOfItemsWithNoData`](../../slicer/showtypeofitemswithnodata/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyCrossFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Set and demonstrate CrossFilterType
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
            Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);

            workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


