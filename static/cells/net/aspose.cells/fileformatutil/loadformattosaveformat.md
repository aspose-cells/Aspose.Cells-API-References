##FileFormatUtil.LoadFormatToSaveFormat
FileFormatUtil method. Converts a LoadFormat value to a SaveFormat value if possible
## FileFormatUtil.LoadFormatToSaveFormat method
Converts a LoadFormat value to a SaveFormat value if possible.
```csharp
public static SaveFormat LoadFormatToSaveFormat(LoadFormat loadFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The load format. |
### Return Value
The save format.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFormatUtilMethodLoadFormatToSaveFormatWithLoadFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
try
{
LoadFormat inputFormat = LoadFormat.Xlsx;
SaveFormat outputFormat = FileFormatUtil.LoadFormatToSaveFormat(inputFormat);
Console.WriteLine($"Converted LoadFormat.{inputFormat} to SaveFormat.{outputFormat}");
string fileExtension = FileFormatUtil.SaveFormatToExtension(outputFormat);
string outputFileName = $"OutputFile_{DateTime.Now.Ticks}.{fileExtension}";
workbook.Save(outputFileName, outputFormat);
Console.WriteLine($"Workbook saved successfully as: {outputFileName}");
}
catch (Exception ex)
{
Console.WriteLine($"Error during conversion or saving: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
