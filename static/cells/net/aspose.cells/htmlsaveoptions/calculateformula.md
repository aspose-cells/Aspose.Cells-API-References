##HtmlSaveOptions.CalculateFormula
HtmlSaveOptions property. Indicates whether to calculate formulas before saving html file
## HtmlSaveOptions.CalculateFormula property
Indicates whether to calculate formulas before saving html file.
```csharp
public bool CalculateFormula { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyCalculateFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data and formulas to the worksheet
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Create HtmlSaveOptions with CalculateFormula set to true
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
CalculateFormula = true
};
// Save the workbook as HTML - formulas will be calculated
workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);
Console.WriteLine("HTML file with calculated formulas created successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
