---
title: PivotTable.CustomListSort
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether consider builtin custom list when sort data
type: docs
url: /net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

Indicates whether consider built-in custom list when sort data

```csharp
public bool CustomListSort { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
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
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Add row field and data field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Enable custom list sorting
            pivotTable.CustomListSort = true;

            // Save the workbook
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


