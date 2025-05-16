---
title: PivotTable.MoveTo
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Moves the PivotTable to a different location in the worksheet
type: docs
url: /net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

Moves the PivotTable to a different location in the worksheet.

```csharp
public void MoveTo(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index. |
| column | Int32 | column index. |

### Examples

```csharp
namespace AsposeCellsExamples.PivotTableMethodMoveToWithInt32Int32Demo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Calculate data to populate the pivot table
            pivotTable.CalculateData();

            try
            {
                // Call MoveTo method with (Int32, Int32) parameters to move the pivot table
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // Calculate data again to update the moved pivot table
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_1}

Moves the PivotTable to a different location in the worksheet.

```csharp
public void MoveTo(string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | String | the dest cell name. |

### Examples

```csharp
// Called: pivot.MoveTo("H16");
public void PivotTable_Method_MoveTo()
{
    Workbook book = new Workbook();
    Worksheet sheet = book.Worksheets[0];
    Cells cells = sheet.Cells;
    cells[0, 0].Value = "fruit";
    cells[1, 0].Value = "grape";
    cells[2, 0].Value = "blueberry";
    cells[3, 0].Value = "kiwi";
    cells[4, 0].Value = "cherry";
    cells[5, 0].Value = "grape";
    cells[6, 0].Value = "blueberry";
    cells[7, 0].Value = "kiwi";
    cells[8, 0].Value = "cherry";

    cells[0, 1].Value = "year";
    cells[1, 1].Value = 2020;
    cells[2, 1].Value = 2020;
    cells[3, 1].Value = 2020;
    cells[4, 1].Value = 2020;
    cells[5, 1].Value = 2021;
    cells[6, 1].Value = 2021;
    cells[7, 1].Value = 2021;
    cells[8, 1].Value = 2021;

    cells[0, 2].Value = "amount";
    cells[1, 2].Value = 50;
    cells[2, 2].Value = 60;
    cells[3, 2].Value = 70;
    cells[4, 2].Value = 80;
    cells[5, 2].Value = 90;
    cells[6, 2].Value = 100;
    cells[7, 2].Value = 110;
    cells[8, 2].Value = 120;

    PivotTableCollection pivots = sheet.PivotTables;

    int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
    PivotTable pivot = pivots[pivotIndex];
    pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
    pivot.AddFieldToArea(PivotFieldType.Column, "year");
    pivot.AddFieldToArea(PivotFieldType.Data, "amount");

    pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

    sheet.RefreshPivotTables();

    Assert.AreEqual(sheet.Cells["B13"].StringValue, "2020");
    Assert.AreEqual(sheet.Cells["A14"].StringValue, "grape");
    book.Save(Constants.PivotTableDestPath + "example.xlsx");

    pivot.MoveTo("H16");
    sheet.RefreshPivotTables();

   // Inconsistent with Excel, the original data should be cleared
    Assert.IsTrue( string.IsNullOrEmpty( sheet.Cells["B13"].StringValue));
    Assert.IsTrue(string.IsNullOrEmpty(sheet.Cells["A14"].StringValue));

    Assert.AreEqual(sheet.Cells["I17"].StringValue, "2020");
    Assert.AreEqual(sheet.Cells["H18"].StringValue, "grape");
    book.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


