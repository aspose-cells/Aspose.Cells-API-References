##FileFormatUtil.FileFormatToSaveFormat
FileFormatUtil method. Converting file format to save format
## FileFormatUtil.FileFormatToSaveFormat method
Converting file format to save format.
```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```
| Parameter | Type | Description |
| --- | --- | --- |
| format | FileFormatType | The file format type. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");
// Get the file format type of the workbook
FileFormatType originalFormat = workbook.FileFormat;
// Convert FileFormatType to SaveFormat
SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);
// Save the workbook using the converted SaveFormat
string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
workbook.Save(outputPath, saveFormat);
Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
