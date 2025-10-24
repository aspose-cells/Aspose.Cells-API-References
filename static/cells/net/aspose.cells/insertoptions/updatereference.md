##InsertOptions.UpdateReference
InsertOptions property. Indicates if references in other worksheets will be updated
## InsertOptions.UpdateReference property
Indicates if references in other worksheets will be updated.
```csharp
public bool UpdateReference { get; set; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class InsertOptionsPropertyUpdateReferenceDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Add a second worksheet and set formulas that reference Sheet1
Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
sheet2.Cells["A1"].Formula = "=Sheet1!A10";
sheet2.Cells["B1"].Formula = "=Sheet1!A5";
// Set formulas in Sheet1
Worksheet sheet1 = wb.Worksheets[0];
sheet1.Cells["A1"].Formula = "=A10";
sheet1.Cells["B1"].Formula = "=A5";
// Create insert options with UpdateReference enabled
InsertOptions iopts = new InsertOptions();
iopts.UpdateReference = true;
// Track formula changes
HashSet<string> changedCells = new HashSet<string>();
iopts.UpdateReference = true;
// Insert rows which will update references in formulas
sheet1.Cells.InsertRows(5, 3, iopts);
// Output the changed cells count
Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
// Display the updated formulas
Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
}
}
}
```
### See Also
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
