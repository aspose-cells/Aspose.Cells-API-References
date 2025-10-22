##SaveOptions.EncryptDocumentProperties
SaveOptions property. Indicates whether encrypt document properties when saving as .xls file. The default value is true
## SaveOptions.EncryptDocumentProperties property
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
```csharp
public bool EncryptDocumentProperties { get; set; }
```
### Remarks
Only for .xls,xlsx,xlsb and xlsm file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some document properties
workbook.BuiltInDocumentProperties.Author = "Test Author";
workbook.BuiltInDocumentProperties.Title = "Test Document";
// Set password protection
workbook.Settings.Password = "password123";
// Save with EncryptDocumentProperties = true (default)
XlsSaveOptions saveOptions1 = new XlsSaveOptions();
saveOptions1.EncryptDocumentProperties = true;
workbook.Save("encrypted_properties.xls", saveOptions1);
// Save with EncryptDocumentProperties = false
XlsSaveOptions saveOptions2 = new XlsSaveOptions();
saveOptions2.EncryptDocumentProperties = false;
workbook.Save("unencrypted_properties.xls", saveOptions2);
// Verify by loading back
Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
