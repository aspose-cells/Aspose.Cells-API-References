---
title: PivotField.IsMultipleItemSelectionAllowed
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether multiple items could be selected in the page field. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

Indicates whether multiple items could be selected in the page field. The default value is false.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsMultipleItemSelectionAllowedDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Add fields
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Access the page field and set multiple selection
            PivotField pageField = pivotTable.PageFields[0];
            pageField.IsMultipleItemSelectionAllowed = true;
            
            // Verify the property was set
            Console.WriteLine("IsMultipleItemSelectionAllowed: " + pageField.IsMultipleItemSelectionAllowed);
            
            // Save the workbook
            workbook.Save("PivotFieldIsMultipleItemSelectionAllowedDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


