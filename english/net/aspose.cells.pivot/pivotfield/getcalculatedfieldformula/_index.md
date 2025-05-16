---
title: PivotField.GetCalculatedFieldFormula
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Get the formula string of the specified calculated field 
type: docs
url: /net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Get the formula string of the specified calculated field .

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GetFormula() method. This method will be removed 12 months later since August 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.PivotFieldMethodGetCalculatedFieldFormulaDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetCalculatedFieldFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Add a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Add a calculated field
            pivotTable.AddCalculatedField("Profit", "Sales*0.1", true);

            // Get the pivot field for the calculated field
            PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
            PivotField calculatedField = dataFields["Profit"];

            try
            {
                // Call the GetCalculatedFieldFormula method
                string formula = calculatedField.GetFormula();

                // Display the result
                Console.WriteLine("Calculated field formula: " + formula);

                // Save the workbook
                workbook.Save("PivotFieldMethodGetCalculatedFieldFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCalculatedFieldFormula method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


