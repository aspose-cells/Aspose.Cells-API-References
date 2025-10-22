##HtmlSaveOptions.ExportFormula
HtmlSaveOptions property. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel please keep the default value
## HtmlSaveOptions.ExportFormula property
Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.
```csharp
public bool ExportFormula { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportFormulaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formula
worksheet.Cells["A1"].PutValue("Value 1");
worksheet.Cells["B1"].PutValue("Value 2");
worksheet.Cells["C1"].Formula = "=A1+B1";
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["C2"].Formula = "=A2+B2";
// Save with ExportFormula = true
HtmlSaveOptions options1 = new HtmlSaveOptions();
options1.ExportFormula = true;
workbook.Save("output_with_formulas.html", options1);
// Save with ExportFormula = false
HtmlSaveOptions options2 = new HtmlSaveOptions();
options2.ExportFormula = false;
workbook.Save("output_without_formulas.html", options2);
// Verify the results
string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");
Console.WriteLine("HTML with formulas contains formula: " +
htmlWithFormulas.Contains("=A2+B2"));
Console.WriteLine("HTML without formulas contains formula: " +
htmlWithoutFormulas.Contains("=A2+B2"));
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
