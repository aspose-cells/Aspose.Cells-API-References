---
title: Class ListColumn
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Tables.ListColumn class. Represents a column in a Table
type: docs
url: /net/aspose.cells.tables/listcolumn/
---
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

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <4; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
ListColumn listColumn = table.ListColumns[4];
listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
listColumn.Formula = "=[A]";
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 3
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
Dim listColumn as ListColumn = table.ListColumns(4);
listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
listColumn.Formula = "=[A]";
workbook.Save("Book1.xlsx")
```

### See Also

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


