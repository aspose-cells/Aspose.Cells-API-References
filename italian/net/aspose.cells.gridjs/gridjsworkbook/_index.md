---
title: GridJsWorkbook
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la classe di ingresso principale per GridJs
type: docs
weight: 80
url: /it/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Rappresenta la classe di ingresso principale per GridJs

```csharp
public class GridJsWorkbook
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | Rappresenta le impostazioni della cartella di lavoro. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso per il file di importazione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | copia immagine o forma nel foglio di lavoro |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | restituisce un messaggio di errore |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson)() | Ottieni json dalla cartella di lavoro |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson_1)(string) | Ottieni json dalla cartella di lavoro |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | Ottieni json dalla cartella di lavoro |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | recupera il json dalla cache tramite uid |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_3)(string) | Importazioni da un file excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile)(Workbook) | Importazioni da cartella di lavoro. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_1)(Stream, GridLoadFormat) | Importazioni da un file excel stream.must fornire loadformat e può impostare GridJsWorkbook.CacheImp per implementare stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_7)(string, string) | Importazioni da un file excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_4)(string, Workbook) | Importazioni da un file excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_2)(Stream, GridLoadFormat, string) | Importazioni da un file excel stream.must fornire loadformat e può impostare GridJsWorkbook.CacheImp per implementare stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_5)(string, Stream, GridLoadFormat) | Importazioni da un file excel stream.must fornire loadformat e può impostare GridJsWorkbook.CacheImp per implementare stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_8)(string, string, string) | Importazioni da un file excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importazioni da un file excel stream.must fornire loadformat e può impostare GridJsWorkbook.CacheImp per implementare stream cache |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | Importa file da json |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | inserisci l'immagine nel foglio di lavoro |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | Applica l'aggiornamento dello stile al file della cache |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | Salva i fogli di lavoro nella cache, il formato di salvataggio si basa sull'estensione del file di nomefile . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile)(Stream) | Salva i fogli di lavoro nello sream, in base al formato del file di origine . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile_1)(string) | Salva i fogli di lavoro nel percorso del file, se il file ha estensione, il formato di salvataggio è basato sull'estensione del file . |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml)(Stream) | Salva i fogli di lavoro nello sream, il formato di salvataggio è html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml_1)(string) | Salva i fogli di lavoro nel percorso del file, il formato di salvataggio è html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf)(Stream) | Salva i fogli di lavoro nello sream, il formato di salvataggio è pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf_1)(string) | Salva i fogli di lavoro nel percorso del file, il formato di salvataggio è pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx)(Stream) | Salva i fogli di lavoro nello sream, il formato di salvataggio è xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx_1)(string) | Salva i fogli di lavoro nel percorso del file, il formato di salvataggio è xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | imposta InterruptMonitor per l'operazione di caricamento per la cartella di lavoro |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | imposta InterruptMonitor per l'operazione di salvataggio per la cartella di lavoro |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | Eseguire l'operazione di aggiornamento |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | Ottieni GridLoadFormat per estensione file |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | Ottieni flusso di immagini dalla cartella di lavoro |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | Ottieni l'URL dell'immagine |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | Genera l'uid per il file |

## Campi

| Nome | Descrizione |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | Implementazione personalizzata per l'archiviazione della cache, se si desidera archiviare la cache in modalità stream, è necessario impostarla e implementarla |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | Implementazione personalizzata per il motore di calcolo ,Se si desidera eseguire un calcolo personalizzato, è necessario impostarlo e implementarlo |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* assemblea [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
