##FormulaParseOptions.LocaleDependent
FormulaParseOptions property. Whether the formula is locale formatted. Default is false
## FormulaParseOptions.LocaleDependent property
Whether the formula is locale formatted. Default is false.
```csharp
public bool LocaleDependent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaParseOptionsPropertyLocaleDependentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
FormulaParseOptions options = new FormulaParseOptions
{
LocaleDependent = true,
R1C1Style = false
};
worksheet.Cells["A1"].SetFormula("=TEXT(TODAY(),\"[$-fr-FR]dddd, dd mmmm yyyy\")", options);
workbook.Save("LocaleDependentFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
