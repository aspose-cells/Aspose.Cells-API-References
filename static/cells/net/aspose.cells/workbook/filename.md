##Workbook.FileName
Workbook property. Gets and sets the current file name
## Workbook.FileName property
Gets and sets the current file name.
```csharp
public string FileName { get; set; }
```
### Remarks
If the file is opened by stream and there are some external formula references, please set the file name.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyFileNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Set the file name property
wb.FileName = "SampleWorkbook.xlsx";
// Add some data to demonstrate functionality
Worksheet sheet = wb.Worksheets[0];
sheet.Cells["A1"].PutValue("Workbook FileName Demo");
sheet.Cells["A2"].PutValue("Current FileName:");
sheet.Cells["B2"].PutValue(wb.FileName);
// Save the workbook
wb.Save(wb.FileName);
Console.WriteLine($"Workbook created with filename: {wb.FileName}");
// Demonstrate changing the filename
Workbook wb2 = new Workbook();
wb2.FileName = "ChangedName.xlsx";
Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
// Demonstrate external link usage
if (wb.Worksheets.ExternalLinks.Count > 0)
{
string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
wb2.FileName = externalSource;
Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
