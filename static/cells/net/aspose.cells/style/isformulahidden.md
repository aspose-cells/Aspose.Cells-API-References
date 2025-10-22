##Style.IsFormulaHidden
Style property. Represents if the formula will be hidden when the worksheet is protected
## Style.IsFormulaHidden property
Represents if the formula will be hidden when the worksheet is protected.
```csharp
public bool IsFormulaHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsFormulaHiddenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style with IsFormulaHidden set to true
Style style = workbook.CreateStyle();
style.IsFormulaHidden = true;
// Apply the style to a cell
cells["A1"].SetStyle(style);
cells["A1"].Formula = "=1+1";
// Create another style with IsFormulaHidden set to false
Style style2 = workbook.CreateStyle();
style2.IsFormulaHidden = false;
// Apply the second style to another cell
cells["B1"].SetStyle(style2);
cells["B1"].Formula = "=2+2";
// Protect the worksheet to see the effect
worksheet.Protect(ProtectionType.All, "password", null);
// Save the workbook
workbook.Save("IsFormulaHiddenDemo.xlsx");
Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
