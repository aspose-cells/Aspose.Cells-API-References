##Class FileFormatInfo
Aspose.Cells.FileFormatInfo class. Contains data returned by FileFormatUtil file format detection methods
## FileFormatInfo class
Contains data returned by [`FileFormatUtil`](../fileformatutil/) file format detection methods.
```csharp
public class FileFormatInfo
```
## Constructors
| Name | Description |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Gets the detected file format. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Returns true if the document is encrypted and requires a password to open. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Gets whether the file is protected by Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Gets the detected load format. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFormatInfoDemo
{
public static void FileFormatInfoExample()
{
// Load a sample file to detect its format
string filePath = "sample.xlsx";
FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);
// Display file format information
Console.WriteLine("File Format Information:");
Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");
// Save the information to a text file
string outputFilePath = "FileFormatInfo.txt";
using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
{
writer.WriteLine("File Format Information:");
writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
}
Console.WriteLine($"File format information saved to {outputFilePath}");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
