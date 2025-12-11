---
title: Enum PivotFieldSubtotalType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFieldSubtotalType enum. Summary description for PivotFieldSubtotalType
type: docs
url: /net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Summary description for PivotFieldSubtotalType.

```csharp
public enum PivotFieldSubtotalType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Represents None subtotal type. |
| Automatic | `1` | Represents Automatic subtotal type. |
| Sum | `2` | Represents Sum subtotal type. |
| Count | `4` | Represents Count subtotal type. |
| Average | `8` | Represents Average subtotal type. |
| Max | `16` | Represents Max subtotal type. |
| Min | `32` | Represents Min subtotal type. |
| Product | `64` | Represents Product subtotal type. |
| CountNums | `128` | Represents Count Nums subtotal type. |
| Stdev | `256` | Represents Standard Deviation subtotal type. |
| Stdevp | `512` | Represents Standard Deviation of a Population subtotal type. |
| Var | `1024` | Represents Variance subtotal type. |
| Varp | `2048` | Represents Variance of a Population subtotal type. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Add a pivot table
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Set subtotal type for the row field
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Refresh and calculate the pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


