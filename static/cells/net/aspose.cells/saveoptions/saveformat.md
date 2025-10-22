##SaveOptions.SaveFormat
SaveOptions property. Gets the save file format
## SaveOptions.SaveFormat property
Gets the save file format.
```csharp
public SaveFormat SaveFormat { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertySaveFormatDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Demonstrate different save formats
SaveOptions[] options = {
new PdfSaveOptions(),
new OoxmlSaveOptions(),
new HtmlSaveOptions()
};
foreach (var saveOptions in options)
{
string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");
string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
workbook.Save(outputPath, saveOptions);
Console.WriteLine($"Saved to: {outputPath}");
}
// Clean up
workbook.Dispose();
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
