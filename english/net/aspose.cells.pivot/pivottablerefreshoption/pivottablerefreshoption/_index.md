---
title: PivotTableRefreshOption.PivotTableRefreshOption
second_title: Aspose.Cells for .NET API Reference
description: PivotTableRefreshOption constructor. Represents the options of refreshing data source of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Represents the options of refreshing data source of the pivot table.

```csharp
public PivotTableRefreshOption()
```

### Examples

```csharp
// Called: PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
public static void PivotTableRefreshOption_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=Sheet1!A1:C5&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Create an instance of PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Refresh the pivot table with the specified options
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotTableRefreshOptionExample.xlsx&quot;);
        }
```

### See Also

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


