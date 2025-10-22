##SaveOptions.CheckExcelRestriction
SaveOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K it will be truncated
## SaveOptions.CheckExcelRestriction property
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
```csharp
public bool CheckExcelRestriction { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyCheckExcelRestrictionDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Disable Excel restriction checking
workbook.Settings.CheckExcelRestriction = false;
// Access first worksheet and cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a string longer than Excel's normal limit
string longString = new string('x', 32767) + " Testing Excel restriction";
// Put the long string in cell A1
cells["A1"].PutValue(longString);
// Configure save options to bypass restrictions
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.CheckExcelRestriction = false;
// Save the workbook
workbook.Save("output_without_restrictions.xlsx", saveOptions);
// Load the saved file with restrictions disabled
LoadOptions loadOptions = new LoadOptions();
loadOptions.CheckExcelRestriction = false;
Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);
// Verify the long string was preserved
string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
Console.WriteLine("Loaded string length: " + loadedValue.Length);
Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
