##FileFormatInfo.LoadFormat
FileFormatInfo property. Gets the detected load format
## FileFormatInfo.LoadFormat property
Gets the detected load format.
```csharp
public LoadFormat LoadFormat { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatInfoPropertyLoadFormatDemo
{
public static void Run()
{
// The path to the documents directory.
string filePath = "data/";
// Detect file format
string fileName = "SAMPLE_XLS_ISSUE.XLS";
var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);
// Load file with correct format
LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
var workbook = new Workbook(filePath + fileName, loadOptions);
// Process the workbook
workbook.Worksheets[0].AutoFitColumns();
workbook.Save(filePath + "output.xlsx");
}
}
}
```
### See Also
* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
