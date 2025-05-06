---
title: PivotTableCalculateOption.RefreshCharts
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCalculateOption property. Indicates whether refreshing charts are based on this pivot table
type: docs
url: /net/aspose.cells.pivot/pivottablecalculateoption/refreshcharts/
---
## PivotTableCalculateOption.RefreshCharts property

Indicates whether refreshing charts are based on this pivot table.

```csharp
public bool RefreshCharts { get; set; }
```

### Examples

```csharp
// Called: RefreshCharts = true,
public static void Property_RefreshCharts()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data for the pivot table
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            sheet.Cells[&quot;B1&quot;].PutValue(&quot;Amount&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Fruit&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(50);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Vegetable&quot;);
            sheet.Cells[&quot;B3&quot;].PutValue(30);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;Fruit&quot;);
            sheet.Cells[&quot;B4&quot;].PutValue(70);
            sheet.Cells[&quot;A5&quot;].PutValue(&quot;Vegetable&quot;);
            sheet.Cells[&quot;B5&quot;].PutValue(40);

            // Add a pivot table to the worksheet
            int pivotIndex = sheet.PivotTables.Add(&quot;A1:B5&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configure the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Create a PivotTableCalculateOption object
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate the pivot table data with the specified options
            pivotTable.CalculateData(calculateOption);

            // Save the workbook
            workbook.Save(&quot;PivotTableCalculateOptionExample.xlsx&quot;);
        }
```

### See Also

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


