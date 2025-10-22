##SaveOptions.ValidateMergedAreas
SaveOptions property. Indicates whether validate merged cells before saving the file
## SaveOptions.ValidateMergedAreas property
Indicates whether validate merged cells before saving the file.
```csharp
public bool ValidateMergedAreas { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyValidateMergedAreasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values and merge cells
worksheet.Cells["A1"].PutValue("Merged Area");
worksheet.Cells["A2"].PutValue("Test");
worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2
// Create save options with ValidateMergedAreas set to true
XlsbSaveOptions saveOptions = new XlsbSaveOptions
{
ValidateMergedAreas = true,
MergeAreas = true
};
// Save the workbook with validation of merged areas
workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);
Console.WriteLine("Workbook saved with merged areas validation.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
