---
title: "Classe WorksheetCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WorksheetCollection. Incapsula una collezione di oggetti Worksheet"
type: docs
url: /it/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Incapsula una collezione di oggetti [`Worksheet`](../worksheet/).

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Rappresenta l'indice del foglio di lavoro attivo quando il foglio elettronico viene aperto. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Rappresenta il nome del foglio di lavoro attivo quando il foglio elettronico viene aperto. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento integrate del foglio elettronico. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento personalizzate del foglio elettronico. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Ottiene i record di formattazione differenziale master. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Rappresenta i collegamenti esterni in una cartella di lavoro. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Ottiene l'elemento [`Worksheet`](../worksheet/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Ottiene la collezione di tutti gli oggetti Name nel foglio elettronico. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Ottiene e imposta la dimensione visualizzata quando il file Workbook è usato come oggetto Ole. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Ottiene tutti i [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Rappresenta i registri di revisione. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Rappresenta tutte le etichette di sensibilità. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Ottiene l'oggetto [`TableStyles`](./tablestyles/). |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Ottiene l'elenco degli autori dei commenti in thread. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Ottiene l'elenco dei riquadri attività. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Ottiene l'elenco dei riquadri attività. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Ottiene e imposta le mappe XML nella cartella di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Aggiunge un foglio di lavoro alla collezione. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Aggiunge un foglio di lavoro alla collezione. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Aggiunge un foglio di lavoro alla collezione. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Copia un gruppo di fogli di lavoro. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Cancella tutti i fogli di lavoro. (2 metodi) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Rimuove le tabelle pivot dal foglio di calcolo. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Crea un oggetto [`Range`](../range/) da un indirizzo dell'intervallo. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Crea un oggetto [`Range`](../range/) da un indirizzo dell'intervallo. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Ottiene l'oggetto Range per nome predefinito. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Ottiene [`Range`](../range/) per nome predefinito o nome della tabella |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Ottiene il foglio di lavoro per nome codice. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Inserisci un foglio di lavoro. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Inserisci un foglio di lavoro. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Obsolete.**) Aggiorna tutte le tabelle pivot e i grafici con la fonte pivot. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Aggiorna tutte le PivotTables nel file Excel. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Aggiorna tutte le PivotTables nel file Excel. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Aggiunge la funzione addin nella cartella di lavoro |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Aggiunge la funzione addin nella cartella di lavoro |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Rimuove l'elemento a un indice specificato. (2 metodi) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Rimuove l'elemento a un nome specificato. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Imposta la dimensione visualizzata quando il file Workbook è usato come oggetto Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Ordina i nomi definiti. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Scambia i due fogli. |

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Aggiungi un nuovo foglio di lavoro alla collezione
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Accedi a un foglio di lavoro esistente per indice
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Accedi a un foglio di lavoro esistente per nome
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Imposta il foglio attivo
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Imposta il nome del foglio attivo
            worksheets.ActiveSheetName = "NewSheet";

            // Aggiorna tutte le tabelle pivot nella cartella di lavoro
            worksheets.RefreshAll();

            // Cancella tutte le tabelle pivot dalla cartella di lavoro
            worksheets.ClearPivottables();

            // Salva la cartella di lavoro
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


