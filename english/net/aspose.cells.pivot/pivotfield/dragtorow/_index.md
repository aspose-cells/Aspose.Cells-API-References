---
title: PivotField.DragToRow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field can be dragged to the row region. The default value is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Indicates whether the specified field can be dragged to the row region. The default value is true.

```csharp
public bool DragToRow { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToRowDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add sample data
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Quarter";
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q3";
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;

            // Create pivot table and get its index
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Get the row field and set DragToRow property
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToRow = true; // This allows the field to be dragged to row area

            // Refresh and calculate data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotFieldDragToRowDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


