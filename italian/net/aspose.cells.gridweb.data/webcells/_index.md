---
title: "Classe WebCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.WebCells."
type: docs
url: /it/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Ottiene il numero di celle. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Restituisce l'elemento Cell all'indice di riga e colonna specificati. (2 indicizzatori) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Ottiene la raccolta di celle unite. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Numero minimo di colonna della cella che contiene dati o stile. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Numero minimo di riga della cella che contiene dati o stile. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Ottiene o imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Cancella il contenuto di un range. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Elimina una colonna. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Elimina una riga. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Elimina un numero di righe. Questo metodo è molto più veloce di DeleteRow quando si esegue l'eliminazione di righe in batch. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Esporta i dati nella raccolta Cells di un WebWorksheet in un nuovo oggetto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Esporta i dati nella collezione Cells in un oggetto array bidimensionale. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Ottiene la didascalia della colonna. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Ottiene se una colonna è di sola lettura. Questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Ottiene la larghezza della colonna specificata |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Ottiene l'enumeratore delle celle |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Ottiene la didascalia della riga. Se la didascalia non è impostata, restituisce una stringa vuota. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Restituisce l'altezza di una riga specificata. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Ottieni lo stato di nascondimento di una riga specificata. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Ottiene il livello di contorno della riga. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Ottiene se una riga è di sola lettura. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Inserisce una nuova colonna nel foglio di lavoro. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Inserisce una nuova riga nel foglio di lavoro. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Inserisce più righe nel foglio di lavoro. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Imposta i bordi per un intervallo di celle. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Imposta la didascalia per la colonna. si prega di notare che questo è un attributo di estensione e non può essere mantenuto nel file Excel |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Imposta una colonna come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Imposta la larghezza della colonna specificata. Il tipo di larghezza accettato è Point, Pixel o Inch. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Imposta la didascalia per la riga. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Imposta l'altezza della riga specificata. Il tipo di larghezza accettato è Point, Pixel o Inch. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Imposta lo stato di nascondimento di una riga specificata. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Imposta il livello di contorno della riga. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Imposta il livello di contorno della riga. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Imposta una riga come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Imposta lo stile a un intervallo specificato di celle. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Imposta lo stile a un intervallo specificato di celle. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per indice di colonna specificato. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per alcuni campi specificati da un array di indici di colonna. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per indice di colonna specificato. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Ordina i dati in ordine ascendente in un intervallo di un WebWorksheet per alcuni campi specificati da un array di indici. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Separa un intervallo specificato di celle unite. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Ottiene il nome della cella in base ai suoi indici di riga e colonna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Ottiene gli indici di riga e colonna della cella in base al suo nome |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Ottiene il nome della colonna in base all'indice della colonna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Ottiene l'indice della colonna in base al nome della colonna. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridCells invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


