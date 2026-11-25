---
title: "Classe Range"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Range. Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo"
type: docs
url: /it/net/aspose.cells/range/
---
## Range class

Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo.

```csharp
public class Range : IEnumerable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Costruttore della classe. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Costruttore della classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Ottiene l'indirizzo dell'intervallo. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Ottiene il conteggio delle colonne nell'intervallo. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Imposta o ottiene la larghezza della colonna di questo intervallo |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Ottiene l'indice della prima colonna dell'intervallo. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Ottiene l'indice della prima riga dell'intervallo. |
| [Height](../../aspose.cells/range/height/) { get; } | Ottiene la larghezza di un intervallo in punti. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Ottiene tutti i collegamenti ipertestuali nell'intervallo. |
| [Item](../../aspose.cells/range/item/) { get; } | Ottiene l'oggetto [`Cell`](../cell/) in questo intervallo. |
| [Left](../../aspose.cells/range/left/) { get; } | Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Ottiene o imposta il nome dell'intervallo. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Ottiene a cosa si riferisce l'intervallo. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Ottiene il conteggio delle righe nell'intervallo. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Imposta o ottiene l'altezza delle righe in questo intervallo |
| [Top](../../aspose.cells/range/top/) { get; } | Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Ottiene e imposta il valore dell'intervallo. |
| [Width](../../aspose.cells/range/width/) { get; } | Ottiene la larghezza di un intervallo in punti. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Ottiene l'oggetto [`Worksheet`](./worksheet/) che contiene questo intervallo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Applica formati a un intero intervallo. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Riempie automaticamente l'intervallo di destinazione. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Riempie automaticamente l'intervallo di destinazione. |
| [Clear](../../aspose.cells/range/clear/)() | Cancella questo intervallo. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Cancella i commenti di questo intervallo. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Cancella il contenuto di questo intervallo. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Cancella i formati di questo intervallo. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Rimuove solo i collegamenti ipertestuali. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Copia i dati (incluse le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Copia l'intervallo con le opzioni incolla speciale. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Copia i dati della cella (incluse le formule) da un intervallo di origine. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Copia le impostazioni di stile da un intervallo di origine. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Copia il valore della cella da un intervallo di origine. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Esporta i dati di questo intervallo in un oggetto DataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Esporta i dati di questo intervallo in un oggetto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Esporta i dati di questo intervallo in un oggetto DataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Ottiene l'oggetto [`Cell`](../cell/) o null in questo intervallo. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Ottiene l'enumeratore per le celle in questo Intervallo. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Ottiene l'intervallo `Range` per offset. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Restituisce un oggetto `Range` che rappresenta l'intersezione rettangolare di due intervalli. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Indica se l'intervallo contiene valori. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Indica se l'intervallo è intersecato. |
| [Merge](../../aspose.cells/range/merge/)() | Combina un intervallo di celle in una singola cella. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Sposta l'intervallo corrente nell'intervallo di destinazione. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Inserisce un valore nell'intervallo; se opportuno il valore sarà convertito in un altro tipo di dati e il formato numerico della cella verrà ripristinato. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Imposta i bordi interni dell'intervallo. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Imposta il bordo esterno attorno a un intervallo di celle. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Imposta il bordo esterno attorno a un intervallo di celle. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Imposta i bordi esterni attorno a un intervallo di celle con lo stesso stile e colore di bordo. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Imposta i bordi esterni attorno a un intervallo di celle con lo stesso stile e colore di bordo. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Imposta i bordi esterni attorno a un intervallo di celle. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Imposta lo stile dell'intervallo. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Applica lo stile della cella. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Converti l'intervallo in HTML. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Converte l'intervallo in immagine. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Converti l'intervallo in valore JSON. |
| override [ToString](../../aspose.cells/range/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
| [Transpose](../../aspose.cells/range/transpose/)() | Trasponi (ruota) i dati dalle righe alle colonne o viceversa. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsoleto.**) Restituisce l'unione di due intervalli. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsoleto.**) Restituisce il risultato dell'unione di due intervalli. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Restituisce il risultato dell'unione di due intervalli. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Separa le celle unite di questo intervallo. |

### Osservazioni

La classe Range indica una regione di un foglio di calcolo Excel. Con questa, puoi formattare e impostare il valore dell'intervallo. E puoi anche copiare semplicemente l'intervallo di Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


