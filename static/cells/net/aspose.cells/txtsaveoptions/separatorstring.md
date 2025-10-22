##TxtSaveOptions.SeparatorString
TxtSaveOptions property. Gets and sets a string value as separator
## TxtSaveOptions.SeparatorString property
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
public class TxtSaveOptionsPropertySeparatorStringDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add test data
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["B1"].PutValue("Column2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
worksheet.Cells["A3"].PutValue(1);
worksheet.Cells["B3"].PutValue(2);
// Save with space separator
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.SeparatorString = " ";
workbook.Save("output_space.txt", saveOptions);
// Save with pipe separator
saveOptions.SeparatorString = "|";
workbook.Save("output_pipe.txt", saveOptions);
// Load the space-separated file to verify
TxtLoadOptions loadOptions = new TxtLoadOptions();
loadOptions.SeparatorString = " ";
Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
Cells cells = loadedWorkbook.Worksheets[0].Cells;
Console.WriteLine("Space-separated values:");
Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
