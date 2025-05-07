---
title: SlicerCache.CrossFilterType
second_title: Aspose.Cells for .NET API Reference
description: SlicerCache property. Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache and how cross filtering is displayed. Read/write
type: docs
url: /net/aspose.cells.slicers/slicercache/crossfiltertype/
---
## SlicerCache.CrossFilterType property

Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write

```csharp
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Slicer Cache Cross Filter Type: " + slicer.SlicerCache.CrossFilterType);
public static void Property_CrossFilterType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add a slicer to the worksheet
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Set the cross filter type for the slicer cache
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;

            // Output the cross filter type
            Console.WriteLine("Slicer Cache Cross Filter Type: " + slicer.SlicerCache.CrossFilterType);

            // Save the workbook
            workbook.Save("SlicerCacheCrossFilterTypeExample.xlsx");
        }
```

### See Also

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


