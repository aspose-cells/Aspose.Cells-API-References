---
title: "Classe WebWorksheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.WebWorksheets."
type: docs
url: /it/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Restituisce un valore che indica se la raccolta ha una dimensione fissa. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Restituisce un valore che indica se l'IList è di sola lettura. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Restituisce un valore che indica se l'accesso a ICollection è sincronizzato (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Restituisce l'elemento Worksheet all'indice specificato. (2 indicizzatori) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Restituisce l'oggetto della raccolta PivotCache |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Restituisce l'oggetto della raccolta pivotTable. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Restituisce un oggetto che può essere usato per sincronizzare l'accesso a ICollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Aggiunge un foglio di lavoro alla collezione. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Aggiunge un oggetto foglio. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Aggiunge un foglio di lavoro alla collezione. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Aggiunge un worksheet alla raccolta e copia i dati da un worksheet esistente. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Aggiunge un worksheet alla raccolta e copia i dati da un worksheet esistente. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Cancella tutti i worksheet. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Indica se la raccolta contiene il foglio. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Copia i contenuti in un array. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Importa da un DataView. Crea automaticamente un foglio con il nome della tabella del DataView. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Importa da un DataView al foglio e alla posizione specificati. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Importa da un file Excel. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Restituisce l'indice del foglio. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Inserisce un foglio all'indice. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Carica i dati da un flusso di file CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Carica i dati da un file CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Carica i dati da un flusso di file HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Carica i dati da un file HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Carica i dati da un flusso di file SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Carica i dati da un file SpreadSheetML. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Rimuove un foglio. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Rimuove un foglio all'indice. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Rimuove l'elemento a un nome specificato. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Esegue tutte le formule delle celle. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Salva i dati in un flusso di file CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Salva i dati in un file CSV. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Salva i dati in un flusso di file HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Salva i dati in un file HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Salva i dati in un flusso di file SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Salva i dati in un file SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Salva i fogli di lavoro in un flusso di file Excel, includendo il flusso di I/O disco o il flusso di memoria. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Salva i fogli di lavoro in un file Excel con formato Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Salva i fogli di lavoro in un file Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Salva i fogli di lavoro in un file Excel. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridWorksheetCollection invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


