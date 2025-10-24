##Style.IsLocked
Style property. Gets or sets a value indicating whether a cell can be modified or not
## Style.IsLocked property
Gets or sets a value indicating whether a cell can be modified or not.
```csharp
public bool IsLocked { get; set; }
```
### Remarks
Locking cells has no effect unless the worksheet is protected.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsLockedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set IsLocked property for a cell
Cell cell = cells["A1"];
Style style = cell.GetStyle();
style.IsLocked = true;
cell.SetStyle(style);
// Protect the worksheet to enforce locking
worksheet.Protect(ProtectionType.All);
// Verify and print the IsLocked status
Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);
// Save the workbook
workbook.Save("IsLockedDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
