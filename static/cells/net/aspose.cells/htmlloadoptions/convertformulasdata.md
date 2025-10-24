##HtmlLoadOptions.ConvertFormulasData
HtmlLoadOptions property. if true convert string to formula when string value starts with character the default value is false
## HtmlLoadOptions.ConvertFormulasData property
if true, convert string to formula when string value starts with character '=',the default value is false.
```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use HtmlLoadOptions.HasFormula property. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
{
public static void Run()
{
// Create an instance of HtmlLoadOptions
HtmlLoadOptions options = new HtmlLoadOptions();
// Set ConvertFormulasData property to true
options.ConvertFormulasData = true;
// Load an HTML file into a Workbook using the specified options
Workbook workbook = new Workbook("input.html", options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some cell values to demonstrate formula conversion
Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);
// Save the workbook to an Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
