##Enum LookInType
Aspose.Cells.LookInType enum. Represents look in type
## LookInType enumeration
Represents look in type.
```csharp
public enum LookInType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Formulas | `0` | Finds the searched object from formula([`Formula`](../cell/formula/)) if the cell is formula, otherwise finds from cell's original value(same with OriginalValues). |
| Values | `1` | Finds object from cell's original value([`Value`](../cell/value/)) and formatted value([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignores cells that are formula. For those cells that are not formula, it is same with Values. |
| Comments | `3` | Finds object from cell's comment only. Ignores those cells that have no comment. |
| OnlyFormulas | `4` | Ignores cells that are not formula. For those cells that are formula, finds the searched object from formula([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Find object from cell's original value only. |
| FormattedValues | `6` | Find object from cell's formatted value([`StringValue`](../cell/stringvalue/)) only. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassLookInTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data and formulas
worksheet.Cells["A1"].PutValue("Test");
worksheet.Cells["B1"].Formula = "=A1";
worksheet.Cells["C1"].PutValue("Contains B1");
// Find cell containing formula with "B1"
FindOptions options = new FindOptions
{
LookInType = LookInType.OnlyFormulas,
LookAtType = LookAtType.Contains
};
Cell foundCell = worksheet.Cells.Find("B1", null, options);
// Output the result
if (foundCell != null)
{
Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
Console.WriteLine($"Cell value: {foundCell.StringValue}");
Console.WriteLine($"Cell formula: {foundCell.Formula}");
}
else
{
Console.WriteLine("Cell not found");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
