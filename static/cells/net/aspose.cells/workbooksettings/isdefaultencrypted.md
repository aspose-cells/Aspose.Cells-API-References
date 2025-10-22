##WorkbookSettings.IsDefaultEncrypted
WorkbookSettings property. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked
## WorkbookSettings.IsDefaultEncrypted property
Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.
```csharp
public bool IsDefaultEncrypted { get; set; }
```
### Remarks
The default value is false now. It's same as MS Excel 2013.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
{
public static void Run()
{
Workbook workbook = new Workbook(FileFormatType.Xlsx);
Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
workbook.Settings.IsDefaultEncrypted = true;
Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
