---
title: PivotField.IsCalculatedField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the this pivot field is calculated field
type: docs
url: /net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

Indicates whether the this pivot field is calculated field.

```csharp
public bool IsCalculatedField { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsCalculatedFieldDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Add a pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Add calculated field
            pivotTable.AddCalculatedField("Profit", "Sales*0.2", true);

            // Check if the field is a calculated field
            PivotField profitField = pivotTable.BaseFields[pivotTable.BaseFields.Count - 1];
            Console.WriteLine("Is Profit field calculated? " + profitField.IsCalculatedField);

            // Save the workbook
            workbook.Save("PivotField_IsCalculatedField_Example.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


