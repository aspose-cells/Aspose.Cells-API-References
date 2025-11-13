---
title: PivotField.GetSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Indicates whether to show specified subtotal for this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Indicates whether to show specified subtotal for this pivot field.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Subtotal type. |

### Return Value

Returns whether showing specified subtotal.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Get the pivot field
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Check if Sum subtotal is enabled
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Check if Average subtotal is enabled
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Enable Sum subtotal
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Verify Sum subtotal is now enabled
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Refresh pivot table to show changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Save the result
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


