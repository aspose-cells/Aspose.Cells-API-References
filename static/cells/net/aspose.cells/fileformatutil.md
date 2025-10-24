##Class FileFormatUtil
Aspose.Cells.FileFormatUtil class. Provides utility methods for converting file format enums to strings or file extensions and back
## FileFormatUtil class
Provides utility methods for converting file format enums to strings or file extensions and back.
```csharp
public class FileFormatUtil
```
## Methods
| Name | Description |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Detects and returns the information about a format of an excel stored in a stream. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Detects and returns the information about a format of an excel stored in a file. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Detects and returns the information about a format of an excel stored in a stream. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Detects and returns the information about a format of an excel stored in a file. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Converts a file name extension into a SaveFormat value. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Converting file format to save format. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Converts a load format enumerated value into a file extension. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Converts a LoadFormat value to a SaveFormat value if possible. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Converts a save format enumerated value into a file extension. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Converts a SaveFormat value to a LoadFormat value if possible. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Detects and returns the information about a format of an excel stored in a stream. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFileFormatUtilDemo
{
public static void Run()
{
string filePath = "example.xlt";
// Detect file format
FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
Console.WriteLine("Detected file format: " + info.FileFormatType);
// Verify file format with Workbook
Workbook workbook = new Workbook(filePath);
Console.WriteLine("Workbook file format: " + workbook.FileFormat);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
