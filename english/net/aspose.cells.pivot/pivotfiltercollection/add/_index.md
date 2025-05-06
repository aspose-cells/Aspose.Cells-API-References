---
title: PivotFilterCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotFilterCollection method. Adds a PivotFilter Object to the specific type
type: docs
url: /net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Adds a PivotFilter Object to the specific type

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | the PivotField index |
| type | PivotFilterType | the PivotFilter type |

### Return Value

the index of the PivotFilter Object in this PivotFilterCollection.

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: int filterIndex = pivotFilters.Add(0, PivotFilterType.Count);
public static void Method_PivotFilterType_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[1, 0].Value = &quot;Grape&quot;;
            worksheet.Cells[2, 0].Value = &quot;Blueberry&quot;;
            worksheet.Cells[3, 0].Value = &quot;Kiwi&quot;;
            worksheet.Cells[4, 0].Value = &quot;Cherry&quot;;
            worksheet.Cells[5, 0].Value = &quot;Grape&quot;;
            worksheet.Cells[6, 0].Value = &quot;Blueberry&quot;;
            worksheet.Cells[7, 0].Value = &quot;Kiwi&quot;;
            worksheet.Cells[8, 0].Value = &quot;Cherry&quot;;

            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Fruit&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Year&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Amount&quot;);

            // Access the PivotFilterCollection
            PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

            // Add a filter to the pivot table
            int filterIndex = pivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotFilters[filterIndex];

            // Set some properties of the filter
            filter.Value1 = &quot;50&quot;;
            filter.Value2 = &quot;100&quot;;
            filter.MeasureFldIndex = 2; // Assuming the measure field index is 2

            // Save the workbook
            workbook.Save(&quot;PivotFilterCollectionExample.xlsx&quot;);
        }
```

### See Also

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


