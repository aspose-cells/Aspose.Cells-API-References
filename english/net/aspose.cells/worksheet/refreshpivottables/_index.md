---
title: Worksheet.RefreshPivotTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Refreshes all the PivotTables in this Worksheet
type: docs
url: /net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Refreshes all the PivotTables in this Worksheet.

```csharp
public void RefreshPivotTables()
```

### Examples

```csharp
// Called: wb.Worksheets[0].RefreshPivotTables();
public void Worksheet_Method_RefreshPivotTables()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    wb.Worksheets[0].RefreshPivotTables();
    Assert.AreEqual("#N/A", wb.Worksheets[0].Cells["H6"].StringValue);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Refreshes all the PivotTables in this Worksheet.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of pivot table. |

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Create a pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Modify source data
            worksheet.Cells["B2"].Value = 25;
            worksheet.Cells["B3"].Value = 30;
            worksheet.Cells["B4"].Value = 35;

            try
            {
                // Create refresh options
                PivotTableRefreshOption options = new PivotTableRefreshOption
                {
                    ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
                };

                // Call the RefreshPivotTables method with options
                bool result = worksheet.RefreshPivotTables(options);

                Console.WriteLine($"Pivot tables refreshed successfully: {result}");
                
                // Access pivot table values through proper methods
                var dataBodyRange = pivotTable.DataBodyRange;
                Console.WriteLine($"Pivot table values after refresh: {worksheet.Cells[dataBodyRange.StartRow, dataBodyRange.StartColumn].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RefreshPivotTables method: {ex.Message}");
            }

            // Save the result
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


