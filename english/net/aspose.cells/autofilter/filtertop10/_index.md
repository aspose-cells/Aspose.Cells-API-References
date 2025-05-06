---
title: AutoFilter.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filter the top 10 item in the list
type: docs
url: /net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filter the top 10 item in the list

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | Boolean | Indicates whether filter from top or bottom |
| isPercent | Boolean | Indicates whether the items is percent or count |
| itemCount | Int32 | The item count |

### Examples

```csharp
// Called: filter.AutoFilter.FilterTop10(0, false, false, 2);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add some data to the worksheet
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;
            cells[5, 0].Value = &quot;grape&quot;;
            cells[6, 0].Value = &quot;blueberry&quot;;
            cells[7, 0].Value = &quot;kiwi&quot;;
            cells[8, 0].Value = &quot;cherry&quot;;

            cells[0, 1].Value = &quot;year&quot;;
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = &quot;amount&quot;;
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Add a PivotTable to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;year&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);

            // Set PivotTable style
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add a PivotFilter to the PivotTable
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionContains);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Refresh and calculate the PivotTable data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotFilterTypeExample.xlsx&quot;);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


