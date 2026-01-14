---
title: PivotTable.Move
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Moves the PivotTable to a different location in the worksheet
type: docs
url: /net/aspose.cells.pivot/pivottable/move/
---
## Move(int, int) {#move}

Moves the PivotTable to a different location in the worksheet.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index. |
| column | Int32 | column index. |

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calculate data to populate the pivot table
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table created at E3");

            try
            {
                // Move the pivot table to new location (row 10, column 5)
                pivotTable.Move(10, 5);
                Console.WriteLine("Pivot table moved to row 10, column 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("PivotTableMethodMoveWithInt32Int32Demo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(string) {#move_1}

Moves the PivotTable to a different location in the worksheet.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | String | the dest cell name. |

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotTable.MoveTo() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // Create pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Add fields to pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Move the pivot table to a new location using cell name
                pivotTable.Move("G10");

                Console.WriteLine("PivotTable moved successfully to G10");
                Console.WriteLine($"New location: {pivotTable.TableRange1.StartRow}, {pivotTable.TableRange1.StartColumn}");

                // Save the workbook
                workbook.Save("PivotTableMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error moving PivotTable: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


