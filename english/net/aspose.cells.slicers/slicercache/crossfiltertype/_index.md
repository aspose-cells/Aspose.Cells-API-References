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
// Called: Console.WriteLine(&amp;quot;Slicer Cache Cross Filter Type: &amp;quot; + slicer.SlicerCache.CrossFilterType);
public static void Property_CrossFilterType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;A1:B4&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Add a slicer to the worksheet
            int slicerIndex = worksheet.Slicers.Add(pivotTable, &quot;A1&quot;, &quot;Category&quot;);
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Set the cross filter type for the slicer cache
            slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;

            // Output the cross filter type
            Console.WriteLine(&quot;Slicer Cache Cross Filter Type: &quot; + slicer.SlicerCache.CrossFilterType);

            // Save the workbook
            workbook.Save(&quot;SlicerCacheCrossFilterTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


