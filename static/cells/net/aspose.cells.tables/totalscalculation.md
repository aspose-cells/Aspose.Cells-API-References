##Enum TotalsCalculation
Aspose.Cells.Tables.TotalsCalculation enum. Determines the type of calculation in the Totals row of the list column
## TotalsCalculation enumeration
Determines the type of calculation in the Totals row of the list column.
```csharp
public enum TotalsCalculation
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Sum | `6` | Represents Sum totals calculation. |
| Count | `2` | Represents Count totals calculation. |
| Average | `1` | Represents Average totals calculation. |
| Max | `4` | Represents Max totals calculation. |
| Min | `5` | Represents Min totals calculation. |
| Var | `8` | Represents Var totals calculation. |
| CountNums | `3` | Represents Count Nums totals calculation. |
| StdDev | `7` | Represents StdDev totals calculation. |
| None | `0` | Represents No totals calculation. |
| Custom | `9` | Represents custom calculation. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TotalsCalculationDemo
{
public static void TotalsCalculationExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Populate the worksheet with some data
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
}
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 4; column++)
{
cells[row, column].PutValue(row * column);
}
}
// Add a table to the worksheet
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
// Show totals row
table.ShowTotals = true;
// Access the fifth column in the table
ListColumn listColumn = table.ListColumns[4];
// Set the TotalsCalculation property to Sum
listColumn.TotalsCalculation = TotalsCalculation.Sum;
// Optionally, set a formula for the column
listColumn.Formula = "=[A]";
// Save the workbook
workbook.Save("TotalsCalculationExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
