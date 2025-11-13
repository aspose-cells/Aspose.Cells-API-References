---
title: PivotTable.Tag
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets a userdefined string that is associated with this PivotTable view
type: docs
url: /net/aspose.cells.pivot/pivottable/tag/
---
## PivotTable.Tag property

Gets and sets a user-defined string that is associated with this PivotTable view.

```csharp
public string Tag { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTagDemo
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
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Add fields to pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Set and demonstrate Tag property
            pivotTable.Tag = "SamplePivotTableTag";
            Console.WriteLine("Pivot Table Tag: " + pivotTable.Tag);

            // Save the workbook
            workbook.Save("PivotTableTagDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


