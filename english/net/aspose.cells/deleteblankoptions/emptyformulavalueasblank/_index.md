---
title: DeleteBlankOptions.EmptyFormulaValueAsBlank
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false
type: docs
url: /net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Remarks

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [`Formula`](../../cell/formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate sample data
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Delete blank rows without considering formula blanks
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Reset data
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Delete blank rows treating formula blanks as empty
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


