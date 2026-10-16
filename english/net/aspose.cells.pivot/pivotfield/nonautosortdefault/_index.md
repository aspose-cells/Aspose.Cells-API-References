---
title: PivotField.NonAutoSortDefault
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort
type: docs
url: /net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use !PivotField.SortSetting.IsSimpleSort property instead. This method will be removed 12 months later since September 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access the first worksheet and pivot table
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Access the first row field in the pivot table
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Set NonAutoSortDefault property to true
            pivotField.NonAutoSortDefault = true;
            
            // Output the property value
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Save the workbook
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


