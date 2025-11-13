---
title: PivotField.IsRepeatItemLabels
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether to repeat labels of the field in the region. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indicates whether to repeat labels of the field in the region. The default value is false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("example.xlsx");

            // Access the worksheet containing the pivot table
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Access the pivot table
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Enable repeating item labels for first row field
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Enable repeating item labels for first column field
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Save the modified workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


