##TxtLoadOptions.SeparatorString
TxtLoadOptions property. Gets and sets a string value as separator
## TxtLoadOptions.SeparatorString property
Gets and sets a string value as separator.
```csharp
public string SeparatorString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertySeparatorStringDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data with custom separator
worksheet.Cells["A1"].PutValue("John&Doe");
worksheet.Cells["B1"].PutValue("30");
worksheet.Cells["A2"].PutValue("Jane&Smith");
worksheet.Cells["B2"].PutValue("25");
// Save with custom separator
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.SeparatorString = "&";
workbook.Save("output.csv", saveOptions);
// Load with the same separator
TxtLoadOptions loadOptions = new TxtLoadOptions();
loadOptions.SeparatorString = "&";
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
