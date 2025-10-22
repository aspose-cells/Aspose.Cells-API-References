##TxtLoadOptions.Separator
TxtLoadOptions property. Gets and sets character separator of text file
## TxtLoadOptions.Separator property
Gets and sets character separator of text file.
```csharp
public char Separator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertySeparatorDemo
{
public static void Run()
{
// Create sample data and save with custom separator
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.Separator = '*';
workbook.Save("output.csv", saveOptions);
// Load the saved file with the same separator
TxtLoadOptions loadOptions = new TxtLoadOptions();
loadOptions.Separator = '*';
Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);
// Verify the loaded data
Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
