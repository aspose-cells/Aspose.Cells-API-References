##FileFormatUtil.DetectFileFormat
FileFormatUtil method. Detects and returns the information about a format of an excel stored in a stream
## DetectFileFormat(Stream) {#detectfileformat}
Detects and returns the information about a format of an excel stored in a stream.
```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
### Return Value
A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Prepare a MemoryStream with workbook data
using (MemoryStream stream = new MemoryStream())
{
// Save workbook to stream in XLSX format
workbook.Save(stream, SaveFormat.Xlsx);
stream.Seek(0, SeekOrigin.Begin); // Reset stream position
try
{
// Detect file format from stream
FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
// Display detection results
Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
}
catch (Exception ex)
{
Console.WriteLine($"Error detecting file format: {ex.Message}");
}
}
// Save the original workbook for verification
workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
}
}
}
```
### See Also
* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DetectFileFormat(Stream, string) {#detectfileformat_1}
Detects and returns the information about a format of an excel stored in a stream.
```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| password | String | The password for encrypted ooxml files. |
### Return Value
A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
{
public static void Run()
{
string sourcePath = "example.xlsx";
using (Stream stream = File.OpenRead(sourcePath))
{
FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
Console.WriteLine("File format: " + info.FileFormatType);
Console.WriteLine("Is encrypted: " + info.IsEncrypted);
Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
}
using (Stream stream = File.OpenRead(sourcePath))
{
FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
Console.WriteLine("File format: " + info.FileFormatType);
Console.WriteLine("Is encrypted: " + info.IsEncrypted);
}
}
}
}
```
### See Also
* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DetectFileFormat(string) {#detectfileformat_2}
Detects and returns the information about a format of an excel stored in a file.
```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
### Return Value
A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodDetectFileFormatWithStringDemo
{
public static void Run()
{
string filePath = "example.xlsx";
FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
Console.WriteLine("Load Format: " + info.LoadFormat);
Console.WriteLine("File Format Type: " + info.FileFormatType);
SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
Console.WriteLine("Save Format: " + saveFormat);
Console.WriteLine("Load Format (converted): " + loadFormat);
}
}
}
```
### See Also
* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DetectFileFormat(string, string) {#detectfileformat_3}
Detects and returns the information about a format of an excel stored in a file.
```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| password | String | The password for encrypted ooxml files. |
### Return Value
A [`FileFormatInfo`](../../fileformatinfo/) object that contains the detected information.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
{
public static void Run()
{
string sourcePath = @"..\..\..\Data\";
// Detect XLSX file format
FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);
// Detect DOCX file format
FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
}
}
}
```
### See Also
* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
