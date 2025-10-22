##FileFormatUtil.ExtensionToSaveFormat
FileFormatUtil method. Converts a file name extension into a SaveFormat value
## FileFormatUtil.ExtensionToSaveFormat method
Converts a file name extension into a SaveFormat value.
```csharp
public static SaveFormat ExtensionToSaveFormat(string extension)
```
| Parameter | Type | Description |
| --- | --- | --- |
| extension | String | The file extension. Can be with or without a leading dot. Case-insensitive. |
### Remarks
If the extension cannot be recognized, returns Unknown.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFormatUtilMethodExtensionToSaveFormatWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("File format demonstration");
try
{
string fileExtension = ".xlsx";
SaveFormat saveFormat = FileFormatUtil.ExtensionToSaveFormat(fileExtension);
Console.WriteLine($"File extension '{fileExtension}' maps to SaveFormat: {saveFormat}");
string verifiedExtension = FileFormatUtil.SaveFormatToExtension(saveFormat);
string outputPath = $"ExtensionConversionDemo{verifiedExtension}";
workbook.Save(outputPath, saveFormat);
Console.WriteLine($"Workbook saved successfully in {saveFormat} format");
}
catch (Exception ex)
{
Console.WriteLine($"Error during format conversion: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
