##Enum NameScopeType
Aspose.Cells.NameScopeType enum. Represents the scope type of defined names
## NameScopeType enumeration
Represents the scope type of defined names.
```csharp
public enum NameScopeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| All | `0` | All defined names. |
| Workbook | `1` | The defined names in the workbook. |
| Worksheet | `2` | The defined names in a worksheet or all worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassNameScopeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
int globalIndex = workbook.Worksheets.Names.Add("GlobalName");
Name globalName = workbook.Worksheets.Names[globalIndex];
globalName.RefersTo = "=Sheet1!$A$1";
int index1 = workbook.Worksheets.Names.Add("SheetLevel1");
Name sheetLevelName1 = workbook.Worksheets.Names[index1];
sheetLevelName1.RefersTo = "=Sheet1!$A$2";
sheetLevelName1.SheetIndex = 0;
int index2 = workbook.Worksheets.Names.Add("SheetLevel2");
Name sheetLevelName2 = workbook.Worksheets.Names[index2];
sheetLevelName2.RefersTo = "=Sheet2!$A$1";
sheetLevelName2.SheetIndex = 1;
Console.WriteLine("Workbook scope names: " +
workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1).Length);
Console.WriteLine("All worksheet scope names: " +
workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
Console.WriteLine("Worksheet scope names (sheet index 0): " +
workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0).Length);
Console.WriteLine("Worksheet scope names (sheet index 1): " +
workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 1).Length);
Console.WriteLine("All defined names: " +
workbook.Worksheets.Names.Filter(NameScopeType.All, -1).Length);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
