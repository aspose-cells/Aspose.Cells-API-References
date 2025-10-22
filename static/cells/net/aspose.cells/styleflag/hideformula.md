##StyleFlag.HideFormula
StyleFlag property. Hide formula setting will be applied
## StyleFlag.HideFormula property
Hide formula setting will be applied.
```csharp
public bool HideFormula { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyHideFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell a1 = worksheet.Cells["A1"];
// Add a formula to cell A1
a1.Formula = "=1+2";
a1.Value = 3; // Display value
// Create a style flag with HideFormula set to true
StyleFlag styleFlag = new StyleFlag();
styleFlag.HideFormula = true;
// Create a style and set IsFormulaHidden to true
Style style = workbook.CreateStyle();
style.IsFormulaHidden = true;
// Apply the style to cell A1 with the style flag
a1.SetStyle(style, styleFlag);
// Protect the worksheet to see the effect of HideFormula
worksheet.Protection.AllowEditingObject = true;
worksheet.Protection.AllowEditingContent = false;
worksheet.Protection.Password = "password";
// Save the workbook
workbook.Save("PropertyHideFormulaDemo.xlsx");
// Verify the formula is hidden
Console.WriteLine("Formula in A1: " + a1.Formula);
Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
