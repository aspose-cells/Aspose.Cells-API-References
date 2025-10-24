##FileFormatUtil.SaveFormatToExtension
FileFormatUtil method. Converts a save format enumerated value into a file extension
## FileFormatUtil.SaveFormatToExtension method
Converts a save format enumerated value into a file extension.
```csharp
public static string SaveFormatToExtension(SaveFormat format)
```
| Parameter | Type | Description |
| --- | --- | --- |
| format | SaveFormat | The save format. |
### Return Value
The returned extension is a lower-case string with a leading dot.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test content");
// Demonstrate SaveFormatToExtension with different formats
SaveOptions[] saveOptions = {
new PdfSaveOptions(),
new XlsSaveOptions(SaveFormat.Excel97To2003),
new OoxmlSaveOptions(SaveFormat.Xlsx),
new OdsSaveOptions()
};
foreach (var options in saveOptions)
{
string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
// Save with the detected extension
string fileName = $"output{extension}";
workbook.Save(fileName, options);
Console.WriteLine($"Saved file: {fileName}");
}
workbook.Dispose();
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
