##Class SpreadsheetLocker
Aspose.Cells.LowCode.SpreadsheetLocker class. Low code api to lock spreadsheet file
## SpreadsheetLocker class
Low code api to lock spreadsheet file.
```csharp
public class SpreadsheetLocker
```
## Methods
| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Locks spreadsheet file with specified settings. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Locks spreadsheet file with specified settings. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Locks spreadsheet file with specified settings. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Locks spreadsheet file with specified settings. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeClassSpreadsheetLockerDemo
{
public static void Run()
{
// Use SpreadsheetLocker to protect the workbook
SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
