---
title: WorksheetCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diWorksheet./worksheet oggetti.
type: docs
weight: 6520
url: /it/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Incapsula una raccolta di[`Worksheet`](../worksheet) oggetti.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Rappresenta l'indice del foglio di lavoro attivo all'apertura del foglio di calcolo. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Rappresenta il nome del foglio di lavoro attivo all'apertura del foglio di calcolo. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Restituisce a[`DocumentProperty`](../../aspose.cells.properties/documentproperty)raccolta che rappresenta tutte le proprietà del documento integrate nel foglio di calcolo. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Restituisce a[`DocumentProperty`](../../aspose.cells.properties/documentproperty) raccolta che rappresenta tutte le proprietà del documento personalizzato del foglio di calcolo. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Ottiene i record di formattazione differenziale principale. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Rappresenta i collegamenti esterni in una cartella di lavoro. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Ottiene il[`Worksheet`](../worksheet) elemento all'indice specificato. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Ottiene e imposta la dimensione visualizzata quando il file cartella di lavoro viene utilizzato come oggetto Ole. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Rappresenta i registri delle revisioni. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Ottiene[`TableStyles`](./tablestyles) oggetto. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Ottiene l'elenco degli autori di commenti in thread. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Ottiene l'elenco dei riquadri attività. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Ottiene l'elenco dei riquadri attività. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Ottiene e imposta le mappe XML nella cartella di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Aggiunge un foglio di lavoro alla raccolta. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Aggiunge un foglio di lavoro alla raccolta. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Aggiunge un foglio di lavoro alla raccolta. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Cancella tutti i fogli di lavoro. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Cancella le tabelle pivot dal foglio di calcolo. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Crea a[`Range`](../range) oggetto da un indirizzo dell'intervallo. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Crea a[`Range`](../range) oggetto da un indirizzo dell'intervallo. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Ottiene l'oggetto Range in base al nome predefinito. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Ottiene[`Range`](../range) per nome predefinito o nome della tabella |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Ottiene il foglio di lavoro in base al nome in codice. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Inserisci un foglio di lavoro. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Inserisci un foglio di lavoro. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Aggiorna tutte le tabelle pivot in WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Aggiunge la funzione di aggiunta nella cartella di lavoro |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Aggiunge la funzione di aggiunta nella cartella di lavoro |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Rimuove l'elemento in corrispondenza di un indice specificato. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Rimuove l'elemento con un nome specificato. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Imposta la dimensione visualizzata quando il file cartella di lavoro viene utilizzato come oggetto Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Ordina i nomi definiti. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Scambia i due fogli. |

### Esempi

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Aggiungi un foglio di lavoro
sheets.Add();

//Cambia il nome di un foglio di lavoro
sheets[0].Name = "First Sheet";

//Imposta il foglio attivo sul secondo foglio di lavoro
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Aggiungi un foglio di lavoro
sheets.Add()

'Modifica il nome di un foglio di lavoro
sheets(0).Name = "First Sheet"

'Imposta il foglio attivo sul secondo foglio di lavoro
sheets.ActiveSheetIndex = 1
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
