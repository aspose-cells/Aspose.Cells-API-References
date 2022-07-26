---
title: Range
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta un intervallo di celle allinterno di un foglio di calcolo.
type: docs
weight: 5030
url: /it/net/aspose.cells/range/
---
## Range class

Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo.

```csharp
public class Range
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Ottiene l'indirizzo dell'intervallo. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Ottiene il conteggio delle colonne nell'intervallo. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Ottiene un oggetto Range che rappresenta l'intera colonna (o colonne) che contiene l'intervallo specificato. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Ottiene un oggetto Range che rappresenta l'intera riga (o righe) che contiene l'intervallo specificato. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Ottiene l'indice della prima colonna dell'intervallo. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Ottiene l'indice della prima riga dell'intervallo. |
| [Height](../../aspose.cells/range/height) { get; } | Ottiene la larghezza di un intervallo in punti. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [Item](../../aspose.cells/range/item) { get; } | Ottiene[`Cell`](../cell) oggetto in questo intervallo. |
| [Left](../../aspose.cells/range/left) { get; } | Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo. |
| [Name](../../aspose.cells/range/name) { get; set; } | Ottiene o imposta il nome dell'intervallo. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Ottiene i riferimenti dell'intervallo a. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Ottiene il conteggio delle righe nell'intervallo. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [Top](../../aspose.cells/range/top) { get; } | Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo. |
| [Value](../../aspose.cells/range/value) { get; set; } | Ottiene e imposta il valore dell'intervallo. |
| [Width](../../aspose.cells/range/width) { get; } | Ottiene la larghezza di un intervallo in punti. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Ottiene il[`Worksheet`](./worksheet) oggetto che contiene questo intervallo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Applica i formati per un intero intervallo. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Tutti riempiono automaticamente l'intervallo di destinazione. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Tutti riempiono automaticamente l'intervallo di destinazione. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Copia i dati (comprese le formule), la formattazione, il disegno di oggetti ecc. da un intervallo di origine. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Copia dell'intervallo con le opzioni speciali di incolla. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Copia i dati della cella (comprese le formule) da un intervallo di origine. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Copia le impostazioni di stile da un intervallo di sorgenti. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Copia il valore della cella da un intervallo di origine. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Esporta i dati in questo intervallo in aDataTable oggetto. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Esporta i dati in questo intervallo in aDataTable oggetto. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Esporta i dati in questo intervallo in aDataTable oggetto. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Ottiene[`Cell`](../cell) oggetto o null in questo intervallo. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Ottiene l'enumeratore per le celle in questo intervallo. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Ottiene[`Range`](../range) intervallo per offset. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Restituisce a[`Range`](../range) oggetto che rappresenta l'intersezione rettangolare di due intervalli. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Indica se l'intervallo è intersecato. |
| [Merge](../../aspose.cells/range/merge)() | Combina un intervallo di celle in una singola cella. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Sposta l'intervallo corrente nell'intervallo più lontano. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Inserisce un valore nell'intervallo, se appropriato il valore verrà convertito in un altro tipo di dati e il formato del numero della cella verrà reimpostato. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Imposta i bordi interni dell'intervallo. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Imposta il bordo del contorno attorno a un intervallo di celle. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Imposta i bordi del contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Imposta i bordi della linea attorno a un intervallo di celle. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Imposta lo stile dell'intervallo. |
| override [ToString](../../aspose.cells/range/tostring)() | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
| [Union](../../aspose.cells/range/union)(Range) | Restituisce l'unione di due intervalli. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Separa le celle unite di questo intervallo. |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
// Ottieni le prime celle del foglio di lavoro.
Cells cells = workbook.Worksheets[0].Cells;
// Crea un intervallo (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Imposta il valore sull'intervallo.
range.Value = "Hello";
//Salva il file Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
'Ottieni le prime celle del foglio di lavoro.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Creare un intervallo (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Imposta il valore sull'intervallo.
range.Value = "Hello"
'Salva il file Excel
workbook.Save("book1.xlsm")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
