##Class TableStyle
Aspose.Cells.Tables.TableStyle class. Represents the table style
## TableStyle class
Represents the table style.
```csharp
public class TableStyle
```
## Properties
| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Gets the name of table style. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Gets all elements of the table style. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleDemo
{
public static void TableStyleExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create styles for the first and last columns
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;
Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.Pattern = BackgroundType.Solid;
lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;
// Define a custom table style name
string tableStyleName = "Custom1";
// Access the table styles collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Add a new table style to the collection
int index1 = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles[index1];
// Access the table style elements collection
TableStyleElementCollection elements = tableStyle.TableStyleElements;
// Add and set style for the first column
index1 = elements.Add(TableStyleElementType.FirstColumn);
TableStyleElement element = elements[index1];
element.SetElementStyle(firstColumnStyle);
// Add and set style for the last column
index1 = elements.Add(TableStyleElementType.LastColumn);
element = elements[index1];
element.SetElementStyle(lastColumnStyle);
// Access the cells of the first worksheet
Cells cells = workbook.Worksheets[0].Cells;
// Populate the first row with column names
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
}
// Populate the rest of the cells with sample data
for (int row = 1; row < 10; row++)
{
for (int column = 0; column < 5; column++)
{
cells[row, column].PutValue(row * column);
}
}
// Add a table to the worksheet
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[index];
// Apply the custom table style to the table
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
table.TableStyleName = tableStyleName;
// Save the workbook
workbook.Save("TableStyleExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
