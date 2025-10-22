##Class ListColumn
Aspose.Cells.Tables.ListColumn class. Represents a column in a Table
## ListColumn class
Represents a column in a Table.
```csharp
public class ListColumn
```
## Properties
| Name | Description |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Gets and sets the formula of the list column. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Indicates whether the fomula is array formula. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Gets and sets the name of the column. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Gets the range of this list column. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Gets and sets the type of calculation in the Totals row of the list column. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Gets and sets the display labels of total row. |
## Methods
| Name | Description |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Gets the formula of this list column. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Gets the formula of totals row of this list column. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Gets the style of the data in this column of the table. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Sets the formula for this list column. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Gets the formula of totals row of this list column. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Sets the style of the data in this column of the table. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class ListColumnDemo
{
public static void ListColumnExample()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
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
// Add a ListObject (table) to the worksheet
ListObjectCollection tables = worksheet.ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
table.ShowTotals = true;
// Access the ListColumn and set its properties
ListColumn listColumn = table.ListColumns[4];
listColumn.TotalsCalculation = TotalsCalculation.Sum;
listColumn.Formula = "=[A]";
listColumn.Name = "CustomColumn";
listColumn.TotalsRowLabel = "Total";
// Save the workbook
workbook.Save("ListColumnExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
