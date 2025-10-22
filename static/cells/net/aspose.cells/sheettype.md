##Enum SheetType
Aspose.Cells.SheetType enum. Specifies the worksheet type
## SheetType enumeration
Specifies the worksheet type.
```csharp
public enum SheetType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| VB | `0` | Visual Basic module |
| Worksheet | `1` |  |
| Chart | `2` | Chart |
| BIFF4Macro | `3` | BIFF4 Macro sheet |
| InternationalMacro | `4` | International Macro sheet |
| Other | `5` |  |
| Dialog | `6` | Dialog worksheet |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassSheetTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Insert a new worksheet of type Worksheet at index 0
Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
// Set the name of the new worksheet
newWorksheet.Name = "InsertedSheet";
// Access cells in the new worksheet and add some data
newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
// Save the workbook
workbook.Save("SheetTypeDemoOutput.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
