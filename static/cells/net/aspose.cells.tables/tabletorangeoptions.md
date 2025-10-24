##Class TableToRangeOptions
Aspose.Cells.Tables.TableToRangeOptions class. Represents the options when converting table to range
## TableToRangeOptions class
Represents the options when converting table to range.
```csharp
public class TableToRangeOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Gets and sets the last row index of the table. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableToRangeOptionsDemo
{
public static void TableToRangeOptionsExample()
{
// Create a new workbook
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
for (int column = 0; column < 5; column++)
{
cells[row, column].PutValue(row * column);
}
}
// Add a ListObject (table) to the worksheet
ListObjectCollection tables = worksheet.ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
// Set some properties of the table
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
// Create an instance of TableToRangeOptions
TableToRangeOptions options = new TableToRangeOptions
{
LastRow = 9 // Set the last row index of the table
};
// Convert the table to a range using the options
table.ConvertToRange(options);
// Save the workbook
workbook.Save("TableToRangeOptionsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
