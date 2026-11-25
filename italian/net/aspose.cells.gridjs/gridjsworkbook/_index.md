---
title: "Classe GridJsWorkbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.GridJsWorkbook. Rappresenta la classe principale di ingresso per GridJs"
type: docs
url: /it/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Rappresenta la classe principale di ingresso per GridJs

```csharp
public class GridJsWorkbook
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Crea una nuova istanza di GridJsWorkbook. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Ottiene/Imposta la directory della cache per la memorizzazione del file di foglio di calcolo. Se non è impostata, utilizzeremo la proprietà statica da [`FileCacheDirectory`](../config/filecachedirectory/) o [`CacheImp`](./cacheimp/) . |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Rappresenta le impostazioni del workbook. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso per l'importazione del file. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Esegue (applica) tutte le operazioni di redazione nella cartella di lavoro rimuovendo le forme di redazione e le loro forme target o cancellando il contenuto dell'intervallo di celle target. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Cancella tutta la cache JSON |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | Cancella la cache JSON in base all'uid (utilizzato per scenari come UpdateCell in cui è presente solo l'uid) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Copia immagine o forma. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Ottiene la stringa del messaggio di errore in formato JSON. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Ottiene la stringa JSON dai dati in memoria, il nome file predefinito nel JSON è: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Ottiene la stringa JSON dai dati in memoria, imposta il nome file di output nel JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Ottieni il JSON del sheet specificato (con cache) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Ottieni il JSON dell'intero workbook (con cache) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Importa il file Excel dal percorso del file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Importa il file Excel dall'oggetto Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Importa il file Excel da un flusso di file con formato di caricamento. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Importa il file Excel dal percorso del file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Importa il file Excel dall'oggetto Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Importa il file Excel da un flusso di file con formato di caricamento e password di apertura. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Importa il file Excel da un flusso di file. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Importa il file Excel dal percorso del file e password di apertura. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importa il file Excel da un flusso di file con formato di caricamento e password di apertura. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Importa il file Excel da una stringa in formato JSON. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Inserisce un'immagine nel foglio di lavoro da un flusso di file o dall'URL (deve essere fornito o il flusso di file o l'URL), oppure inserisce una forma quando p.type è uno di AutoShapeType. |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Genera JSON dal Workbook in memoria e lo scrive nello stream specificato. Opzionalmente memorizza nella cache il JSON generato per un recupero più rapido successivo. Differenze principali rispetto a JsonToStreamByUid: - Questo metodo utilizza lo stato attuale del Workbook in memoria (campo wb) - JsonToStreamByUid ricarica il Workbook dai file di cache .cells su disco - Usa questo metodo quando vuoi esportare lo stato corrente del workbook dopo le modifiche - Usa JsonToStreamByUid quando devi rigenerare JSON da uno stato di file precedentemente memorizzato nella cache. Comportamento della cache (quando uid è fornito): - Controlla la cache JSON prima di generare (memoria L1 + disco L2) - In caso di cache miss, genera JSON dal workbook in memoria - Salva il JSON generato nella cache per richieste future |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Recupera la stringa JSON del file dalla cache usando l'ID unico specificato, imposta il nome file di output nel JSON e scrivila nello stream. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Recupera la stringa JSON del foglio specificato nel file dalla cache usando l'ID unico specificato e scrivila nello stream. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Applica un aggiornamento batch ai dati in memoria. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Esegue la redazione di un file Excel basata su un array di operazioni JSON. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Salva i dati in memoria nel file di cache con il nome file specificato e imposta anche la password di apertura; il formato di salvataggio è basato sull'estensione del nome file. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Salva i dati in memoria nello stream, basato sul formato del file originale. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Salva i dati in memoria nel percorso del file; se il file ha un'estensione, il formato di salvataggio è basato sull'estensione del file. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Salva i dati in memoria nello stream, il formato di salvataggio è html. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Salva i dati in memoria nel percorso del file, il formato di salvataggio è html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Salva i dati in memoria nello stream, il formato di salvataggio è pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Salva i dati in memoria nel percorso del file, il formato di salvataggio è pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Salva i dati in memoria nello stream, il formato di salvataggio è xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Salva i dati in memoria nel percorso del file, il formato di salvataggio è xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Imposta InterruptMonitor per l'operazione di caricamento. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Imposta InterruptMonitor per l'operazione di salvataggio. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Imposta la trasparenza delle forme di redazione nella cartella di lavoro. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Traduci tutti i valori stringa nella lingua di destinazione nel foglio di lavoro |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Applica l'operazione di aggiornamento. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Ottiene il formato di caricamento in base all'estensione del file |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Ottieni lo stream dell'immagine. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Ottiene l'URL dell'immagine. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Genera un nuovo ID univoco per la cache dei file utilizzando il nome file fornito. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Imposta l'URL dell'azione di recupero dell'immagine di base dal controller. |

## Campi

| Nome | Descrizione |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Implementazione personalizzata per l'archiviazione della cache. Se desideri memorizzare la cache in modalità stream, devi impostarla e implementarla. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Implementazione personalizzata per il motore di calcolo. Se desideri eseguire calcoli personalizzati, devi impostarla e implementarla. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | valore costante per il tipo dell'immagine |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Ottiene/Imposta il monitor di aggiornamento per tracciare l'operazione di aggiornamento |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


