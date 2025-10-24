##FormulaParseOptions.CheckAddIn
FormulaParseOptions property. Whether check addins in existing external links of current workbook for user defined function without external link. Default is trueif user defined function matches one addin in existing external links then take it as the addin
## FormulaParseOptions.CheckAddIn property
Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).
```csharp
public bool CheckAddIn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaParseOptionsPropertyCheckAddInDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Register add-in function
wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);
// Without CheckAddIn=false - formula will be converted to add-in format
cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);
// With CheckAddIn=false - formula remains unchanged
cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
}
}
}
```
### See Also
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
