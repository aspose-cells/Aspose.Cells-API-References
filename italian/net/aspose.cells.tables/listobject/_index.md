---
title: ListObject
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta un oggetto elenco in un foglio di lavoro. Loggetto ListObject è un membro della raccolta ListObjects. La raccolta ListObjects contiene tutti gli oggetti elenco su un foglio di lavoro.
type: docs
weight: 5820
url: /it/net/aspose.cells.tables/listobject/
---
## ListObject class

Rappresenta un oggetto elenco in un foglio di lavoro. L'oggetto ListObject è un membro della raccolta ListObjects. La raccolta ListObjects contiene tutti gli oggetti elenco su un foglio di lavoro.

```csharp
public class ListObject
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | Ottiene e imposta la descrizione alternativa. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | Ottiene e imposta il testo alternativo. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | Ottiene il filtro automatico. |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | Ottiene e imposta il commento della tabella. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | Ottiene l'intervallo di dati di ListObject. |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | Ottiene il tipo di origine dati della tabella. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | Ottiene e imposta il nome visualizzato. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | Ottiene la colonna finale dell'intervallo. |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | Ottiene la riga finale dell'intervallo. |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | Ottiene ListColumns di ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | Ottiene la QueryTable collegata. |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | Ottiene e imposta se questo ListObject mostra la riga di intestazione. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | Indica se è stata applicata la formattazione della striscia di colonna. |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | Indica se alla prima colonna della tabella deve essere applicato lo stile. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | Indica se lo stile deve essere applicato all'ultima colonna della tabella. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | Indica se è stata applicata la formattazione della striscia di riga. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | Ottiene e imposta se questo ListObject mostra la riga totale. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | Ottiene la colonna iniziale dell'intervallo. |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | Ottiene la riga iniziale dell'intervallo. |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | Ottiene e imposta il nome dello stile della tabella. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | Ottiene e lo stile tabella integrato. |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | Ottiene un[`XmlMap`](./xmlmap)utilizzato per questo elenco. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | Applica lo stile della tabella all'intervallo. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | Converti la tabella in intervallo. |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | Converti la tabella in intervallo. |
| [Filter](../../aspose.cells.tables/listobject/filter)() | Filtra la tabella. |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | Inserisci il valore nella cella. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | Ridimensiona l'intervallo dell'oggetto elenco. |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | Aggiorna il nome di tutte le colonne dell'elenco dal foglio di lavoro. |

### Esempi

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

### Guarda anche

* spazio dei nomi [Aspose.Cells.Tables](../../aspose.cells.tables)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
