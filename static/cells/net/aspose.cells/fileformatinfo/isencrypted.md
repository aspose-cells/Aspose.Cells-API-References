##FileFormatInfo.IsEncrypted
FileFormatInfo property. Returns true if the document is encrypted and requires a password to open
## FileFormatInfo.IsEncrypted property
Returns true if the document is encrypted and requires a password to open.
```csharp
public bool IsEncrypted { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatInfoPropertyIsEncryptedDemo
{
public static void Run()
{
// Detect file format of an unencrypted file
FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);
// Detect file format of an encrypted file
FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);
// Load encrypted file with password
LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
loadOptions.Password = "password";
Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
Console.WriteLine("Encrypted file loaded successfully");
}
}
}
```
### See Also
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
