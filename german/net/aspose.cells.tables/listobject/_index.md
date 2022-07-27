---
title: ListObject
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert ein Listenobjekt auf einem Arbeitsblatt. Das ListObject-Objekt ist ein Mitglied der ListObjects-Auflistung. Die ListObjects-Auflistung enthält alle Listenobjekte auf einem Arbeitsblatt.
type: docs
weight: 5820
url: /de/net/aspose.cells.tables/listobject/
---
## ListObject class

Repräsentiert ein Listenobjekt auf einem Arbeitsblatt. Das ListObject-Objekt ist ein Mitglied der ListObjects-Auflistung. Die ListObjects-Auflistung enthält alle Listenobjekte auf einem Arbeitsblatt.

```csharp
public class ListObject
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Ruft die alternative Beschreibung ab und legt sie fest. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Ruft den alternativen Text ab und setzt ihn. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Ruft den automatischen Filter ab. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Liest und setzt den Kommentar der Tabelle. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Ruft den Datenbereich des Listenobjekts ab. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Ruft den Datenquellentyp der Tabelle ab. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Ruft den Anzeigenamen ab und legt ihn fest. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Ruft die letzte Spalte des Bereichs ab. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Ruft die Endzeile des Bereichs ab. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Ruft ListColumns des ListObject ab. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Ruft die verknüpfte QueryTable ab. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Ruft ab und legt fest, ob dieses ListObject die Kopfzeile anzeigt. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Gibt an, ob der Stil auf die erste Spalte in der Tabelle angewendet werden soll. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Gibt an, ob der Stil auf die letzte Spalte in der Tabelle angewendet werden soll. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Ruft ab und legt fest, ob dieses ListObject die Gesamtzeile anzeigt. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Ruft die Startspalte des Bereichs ab. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Ruft die Anfangszeile des Bereichs ab. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Ruft den Namen des Tabellenstils ab und legt ihn fest. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Gets und der integrierte Tabellenstil. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Ruft ein[`XmlMap`](./xmlmap)für diese Liste verwendet. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Wenden Sie den Tabellenstil auf den Bereich an. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Wandeln Sie die Tabelle in einen Bereich um. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Wandeln Sie die Tabelle in einen Bereich um. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Tabelle filtern. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Tragen Sie den Wert in die Zelle ein. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Größe des Bereichs des Listenobjekts ändern. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Aktualisiert den Namen aller Listenspalten aus dem Arbeitsblatt. |

### Beispiele

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

### Siehe auch

* namensraum [Aspose.Cells.Tables](../../aspose.cells.tables)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
