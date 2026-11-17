---
title: "Classe WorksheetCollection"
linktitle: "WorksheetCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe WorksheetCollection. Incapsula l'oggetto che rappresenta worksheetcollection in Go."
type: docs
weight: 200
url: /it/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Incapsula una raccolta di oggetti <see cref="Worksheet"/>.

```go

type WorksheetCollection struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Restituisce l'elenco dei riquadri delle attività. |
| [GetWebExtensions](./getwebextensions/) | Restituisce l'elenco dei riquadri delle attività. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Restituisce l'elenco degli autori dei commenti in thread. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [CreateRange](./createrange/) | Crea un oggetto Range da un indirizzo dell'intervallo. |
| [CreateUnionRange](./createunionrange/) | Crea un oggetto Range da un indirizzo dell'intervallo. |
| [GetNames](./getnames/) | Restituisce la raccolta di tutti gli oggetti Name nel foglio di calcolo. |
| [Get_Int](./get_int/) | Restituisce l'elemento Worksheet all'indice specificato. |
| [Get_String](./get_string/) | Restituisce l'elemento Worksheet con il nome specificato. |
| [GetSheetByCodeName](./getsheetbycodename/) | Restituisce il foglio di lavoro per nome codice. |
| [GetActiveSheetName](./getactivesheetname/) | Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo viene aperto. |
| [SetActiveSheetName](./setactivesheetname/) | Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo viene aperto. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo viene aperto. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo viene aperto. |
| [SortNames](./sortnames/) | Ordina i nomi definiti. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Inserisci un foglio di lavoro. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Inserisci un foglio di lavoro. |
| [Add_SheetType](./add_sheettype/) | Aggiunge un foglio di lavoro alla raccolta. |
| [SwapSheet](./swapsheet/) | Scambia i due fogli. |
| [Add](./add/) | Aggiunge un foglio di lavoro alla raccolta. |
| [Add_String](./add_string/) | Aggiunge un foglio di lavoro alla raccolta. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Aggiunge la funzione addin nella cartella di lavoro |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Aggiunge la funzione addin nella cartella di lavoro |
| [RemoveAt_String](./removeat_string/) | Rimuove l'elemento con un nome specificato. |
| [RemoveAt_Int](./removeat_int/) | Rimuove l'elemento all'indice specificato. |
| [Clear](./clear/) | Cancella tutti i fogli di lavoro. |
| [AddCopy_String](./addcopy_string/) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [AddCopy_Int](./addcopy_int/) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Copia un gruppo di fogli di lavoro. |
| [GetDxfs](./getdxfs/) | Restituisce i record di formattazione differenziale master. |
| [GetRangeByName_String](./getrangebyname_string/) | Ottiene l'oggetto Range per nome predefinito. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Ottiene Range per nome predefinito o nome della tabella |
| [GetNamedRanges](./getnamedranges/) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [GetXmlMaps](./getxmlmaps/) | Ottiene e imposta le mappe XML nella cartella di lavoro. |
| [SetXmlMaps](./setxmlmaps/) | Ottiene e imposta le mappe XML nella cartella di lavoro. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento integrate del foglio di calcolo. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo. |
| [GetOleSize](./getolesize/) | Ottiene e imposta la dimensione visualizzata quando il file della cartella di lavoro è usato come oggetto OLE. |
| [SetOleSize_Object](./setolesize_object/) | Ottiene e imposta la dimensione visualizzata quando il file della cartella di lavoro è usato come oggetto OLE. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Imposta la dimensione visualizzata quando il file della cartella di lavoro è usato come oggetto OLE. |
| [GetExternalLinks](./getexternallinks/) | Rappresenta i collegamenti esterni in una cartella di lavoro. |
| [GetPivotCaches](./getpivotcaches/) | Ottiene tutti i PivotCache. |
| [GetTableStyles](./gettablestyles/) | Ottiene l'oggetto TableStyles. |
| [ClearPivottables](./clearpivottables/) | Cancella le tabelle pivot dal foglio di calcolo. |
| [GetRevisionLogs](./getrevisionlogs/) | Rappresenta i registri delle revisioni. |
| [RefreshPivotTables](./refreshpivottables/) | Aggiorna tutte le PivotTable nel file Excel. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Aggiorna tutte le PivotTable nel file Excel. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Rappresenta tutte le etichette di sensibilità. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
