---
title: PivotTableCalculateOption.RefreshData
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCalculateOption property. Indicates whether refreshing data source of the pivottable
type: docs
url: /net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indicates whether refreshing data source of the pivottable.

```csharp
public bool RefreshData { get; set; }
```

### Examples

```csharp
// Called: RefreshData = true,
public static void Property_RefreshData()
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

            // Add a PivotTable to the worksheet
            int pivotTableIndex = worksheet.PivotTables.Add(&quot;A1:B4&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Add fields to the PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Category&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Value&quot;);

            // Set the ReserveMissingPivotItemType option
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate the PivotTable with the specified options
            pivotTable.CalculateData(calculateOption);

            // Refresh the PivotTable
            pivotTable.RefreshData();

            // Save the workbook
            workbook.Save(&quot;ReserveMissingPivotItemTypeExample.xlsx&quot;);
        }
```

### See Also

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


