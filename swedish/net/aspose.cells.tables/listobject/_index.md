---
title: ListObject
second_title: Aspose.Cells för .NET API-referens
description: Representerar ett listobjekt på ett kalkylblad. ListObject-objektet är en medlem av ListObjects-samlingen. ListObjects-samlingen innehåller alla listobjekt på ett kalkylblad.
type: docs
weight: 5820
url: /sv/net/aspose.cells.tables/listobject/
---
## ListObject class

Representerar ett listobjekt på ett kalkylblad. ListObject-objektet är en medlem av ListObjects-samlingen. ListObjects-samlingen innehåller alla listobjekt på ett kalkylblad.

```csharp
public class ListObject
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Hämtar och ställer in den alternativa beskrivningen. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Hämtar och ställer in den alternativa texten. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Får autofilter. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Hämtar och ställer in tabellens kommentar. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Hämtar dataintervallet för ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Hämtar datakällans typ för tabellen. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Hämtar och ställer in visningsnamnet. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Hämtar slutkolumnen i intervallet. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Hämtar slutraden i intervallet. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Hämtar ListColumns för ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Hämtar den länkade frågetabellen. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Hämtar och ställer in om detta ListObject visar rubrikrad. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Indikerar om formatering av kolumnrand används. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Anger om den första kolumnen i tabellen ska ha stilen tillämpad. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Anger om den sista kolumnen i tabellen ska ha stilen tillämpad. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Indikerar om radrandsformatering tillämpas. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Hämtar och ställer in om detta ListObject visar total rad. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Hämtar startkolumnen för intervallet. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Hämtar startraden för intervallet. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Hämtar och ställer in tabellstilens namn. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Gets och den inbyggda tabellstilen. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Får en[`XmlMap`](./xmlmap)används för den här listan. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Tillämpa tabellformatet på intervallet. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Konvertera tabellen till intervall. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Konvertera tabellen till intervall. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Filtrera tabellen. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Sätt värdet i cellen. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Ändra storlek på listobjektets intervall. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Uppdaterar namnet på alla listkolumner från kalkylbladet. |

### Exempel

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

### Se även

* namnutrymme [Aspose.Cells.Tables](../../aspose.cells.tables)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
