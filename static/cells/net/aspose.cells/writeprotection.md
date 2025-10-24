##Class WriteProtection
Aspose.Cells.WriteProtection class. Specifies write protection settings for a workbook
## WriteProtection class
Specifies write protection settings for a workbook.
```csharp
public class WriteProtection
```
## Properties
| Name | Description |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Gets and sets the author. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Indicates whether this workbook is write protected. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Sets the protected password to modify the file. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Indicates if the Read Only Recommended option is selected. |
## Methods
| Name | Description |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Returns true if the specified password is the same as the write-protection password the file was protected with. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WriteProtectionDemo
{
public static void WriteProtectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the workbook's settings
WorkbookSettings settings = workbook.Settings;
// Access the write protection settings
WriteProtection writeProtection = settings.WriteProtection;
// Set the author of the write protection
writeProtection.Author = "John Doe";
// Set the password for write protection
writeProtection.Password = "password123";
// Set the recommend read-only option
writeProtection.RecommendReadOnly = true;
// Check if the workbook is write protected
bool isWriteProtected = writeProtection.IsWriteProtected;
Console.WriteLine("Is Write Protected: " + isWriteProtected);
// Validate the password
bool isValidPassword = writeProtection.ValidatePassword("password123");
Console.WriteLine("Is Valid Password: " + isValidPassword);
// Save the workbook
workbook.Save("WriteProtectionExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
