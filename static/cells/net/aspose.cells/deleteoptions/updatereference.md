##DeleteOptions.UpdateReference
DeleteOptions property. Indicates if update references in other worksheets
## DeleteOptions.UpdateReference property
Indicates if update references in other worksheets.
```csharp
public bool UpdateReference { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteOptionsPropertyUpdateReferenceDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formulas
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["B1"].PutValue(20);
worksheet.Cells["C1"].Formula = "=A1+B1";
worksheet.Cells["A2"].PutValue(30);
worksheet.Cells["B2"].PutValue(40);
worksheet.Cells["C2"].Formula = "=A2+B2";
// Create delete options with UpdateReference set to true
DeleteOptions deleteOptions = new DeleteOptions();
deleteOptions.UpdateReference = true;
// Delete column A which is referenced in formulas
worksheet.Cells.DeleteColumns(0, 1, deleteOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
