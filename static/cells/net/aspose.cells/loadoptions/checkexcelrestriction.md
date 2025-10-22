##LoadOptions.CheckExcelRestriction
LoadOptions property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
## LoadOptions.CheckExcelRestriction property
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.
```csharp
public bool CheckExcelRestriction { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyCheckExcelRestrictionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Disable Excel restrictions checking
workbook.Settings.CheckExcelRestriction = false;
// Access first worksheet and cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a string longer than Excel's normal limit (32767 characters)
string longString = new string('x', 32767) + " Testing Excel restriction";
// Put the long string in cell A1
cells["A1"].PutValue(longString);
// Save with restrictions checking disabled
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.CheckExcelRestriction = false;
workbook.Save("output.xlsx", saveOptions);
// Load with restrictions checking disabled
LoadOptions loadOptions = new LoadOptions();
loadOptions.CheckExcelRestriction = false;
Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
// Verify the long string was preserved
string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
Console.WriteLine("String length: " + loadedValue.Length);
Console.WriteLine("String matches: " + loadedValue.Equals(longString));
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
