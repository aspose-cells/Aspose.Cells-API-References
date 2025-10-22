##FileFormatInfo.FileFormatType
FileFormatInfo property. Gets the detected file format
## FileFormatInfo.FileFormatType property
Gets the detected file format.
```csharp
public FileFormatType FileFormatType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatInfoPropertyFileFormatTypeDemo
{
public static void Run()
{
// Example 1: Detect Excel 97-2003 format
string excelFile = "sample.xls";
FileFormatInfo info = FileFormatUtil.DetectFileFormat(excelFile);
Console.WriteLine("File Format Type: " + info.FileFormatType);
Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
// Example 2: Detect OOXML format
string xlsxFile = "sample.xlsx";
info = FileFormatUtil.DetectFileFormat(xlsxFile);
Console.WriteLine("File Format Type: " + info.FileFormatType);
Console.WriteLine("Is Encrypted: " + info.IsEncrypted);
}
}
}
```
### See Also
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
