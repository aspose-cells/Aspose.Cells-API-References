##WorkbookSettings.IsEncrypted
WorkbookSettings property. Gets a value that indicates whether a password is required to open this workbook
## WorkbookSettings.IsEncrypted property
Gets a value that indicates whether a password is required to open this workbook.
```csharp
public bool IsEncrypted { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsEncryptedDemo
{
public static void Run()
{
// Example 1: Check if a password-protected workbook is encrypted
string encryptedFilePath = "encrypted.xlsx";
var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");
// Example 2: Check if a normal workbook is encrypted
string normalFilePath = "normal.xlsx";
var normalWorkbook = new Workbook(normalFilePath);
Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");
// Example 3: Create and save an encrypted workbook
var newWorkbook = new Workbook();
newWorkbook.Settings.Password = "12345";
newWorkbook.Save("new_encrypted.xlsx");
Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
