---
title: PivotField.Ungroup
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Ungroup the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Ungroup the pivot field.

```csharp
public void Ungroup()
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the first pivot table
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ungroup the first column field
            pivotTable.ColumnFields[0].Ungroup();
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


