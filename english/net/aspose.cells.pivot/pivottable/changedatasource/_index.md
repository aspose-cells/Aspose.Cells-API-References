---
title: PivotTable.ChangeDataSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Change data source of the pivottable
type: docs
url: /net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

Change data source of the pivottable.

```csharp
public void ChangeDataSource(string[] source)
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Create a pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Prepare new data source
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // Change the data source of the pivot table
                pivotTable.ChangeDataSource(newDataSource);

                // Refresh the pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


