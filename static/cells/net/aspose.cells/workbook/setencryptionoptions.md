##Workbook.SetEncryptionOptions
Workbook method. Set Encryption Options
## Workbook.SetEncryptionOptions method
Set Encryption Options.
```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```
| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | EncryptionType | The encryption type. |
| keyLength | Int32 | The key length. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some data to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Encryption");
// Set password and encryption options
workbook.Settings.Password = "1234";
workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
// Save the encrypted workbook
workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
// Verify by loading the encrypted workbook
LoadOptions loadOptions = new LoadOptions();
loadOptions.Password = "1234";
Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
Console.WriteLine("Workbook encrypted and loaded successfully.");
}
}
}
```
### See Also
* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
