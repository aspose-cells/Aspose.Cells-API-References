---
title: ListObject
second_title: Aspose.Cells for .NET API Reference
description: Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.
type: docs
url: /net/aspose.cells.tables/listobject/
---
## ListObject class

Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.

```csharp
public class ListObject
```

## Properties

| Name | Description |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Gets and sets the alternative description. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Gets and sets the alternative text. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Gets auto filter. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Gets and sets the comment of the table. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Gets the data range of the ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Gets the data source type of the table. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Gets and sets the display name. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Gets the end column of the range. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Gets the end row of the range. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Gets ListColumns of the ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Gets the linked QueryTable. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Gets and sets whether this ListObject show header row. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Indicates whether column stripe formatting is applied. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Indicates whether the first column in the table should have the style applied. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Indicates whether the last column in the table should have the style applied. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Indicates whether row stripe formatting is applied. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Gets and sets whether this ListObject show total row. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Gets the start column of the range. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Gets the start row of the range. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Gets and sets the table style name. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Gets and the built-in table style. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Gets an [`XmlMap`](./xmlmap) used for this list. |

## Methods

| Name | Description |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Apply the table style to the range. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Convert the table to range. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Convert the table to range. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Filter the table. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Put the value to the cell. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Resize the range of the list object. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Updates all list columns' name from the worksheet. |

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
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### See Also

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
