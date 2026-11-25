---
title: "Classe GridJsOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.GridJsOptions. Rappresenta tutte le opzioni di caricamento per GridJs"
type: docs
url: /it/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Rappresenta tutte le opzioni di caricamento per GridJs

```csharp
public class GridJsOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file, il valore predefinito è false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file, il valore predefinito è false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Ottiene/Imposta se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili/bordi per ridurre il tempo di caricamento. Il valore predefinito è true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Ottiene/Imposta il nome base dell'URL di route per il controller GridJs. Il valore predefinito è GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Ottiene/Imposta le PdfSaveOptions personalizzate per l'esportazione PDF. Se impostato, verrà usato al posto delle opzioni predefinite. Il valore predefinito è null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Ottiene/Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Ottiene/Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Ottiene/Imposta se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs emetterà solo immagini/forme dei grafici e non richiederà il rendering lato client. Il valore predefinito è true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Ottiene/Imposta la directory della cache per memorizzare il file del foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Ottiene/Imposta le cartelle dei font per i caratteri nelle immagini/forme renderizzate |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Ottiene/Imposta se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, allora non mostreremo questa riga/colonna quando questo valore è true. Il valore predefinito è true. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Ottiene/Imposta se supportare la modifica collaborativa, il valore predefinito è false. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Ottiene/Imposta se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro. Se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Ottiene/Imposta se GridJs viene eseguito all'interno di un host WebAssembly del browser anziché di un processo server. Quando è true, non viene utilizzato alcun percorso FileCacheDirectory / disco / thread di interruzione, e la cache dei file deve provenire da CacheImp, poiché un host browser non ha disco locale. Seleziona i percorsi di codice a runtime, quindi un unico Aspose.Cells.GridJs.dll serve entrambi gli host. Il valore predefinito è false. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Ottiene/Imposta le opzioni di configurazione della cache JSON. Controlla il comportamento della cache di memoria (L1) e disco (L2) per il JSON del workbook generato. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Ottiene/Imposta se caricare solo il foglio di lavoro attivo, il valore predefinito è false. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Ottiene/Imposta i secondi massimi di timeout durante il salvataggio in PDF. Il valore predefinito è 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Ottiene/Imposta il conteggio totale di forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Ottiene/Imposta la larghezza o altezza massima per una forma o un'immagine; GridJs ignorerà la forma o l'immagine con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Ottiene/Imposta il conteggio totale di forme o immagini visualizzate nella cartella di lavoro, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Ottiene/Imposta le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Ottiene/Imposta la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) Il percorso predefinito sarà "_piccache" all'interno di FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Ottiene/Imposta se verificare se le immagini hanno la stessa origine, il valore predefinito è true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Ottiene/Imposta se salvare il file HTML come archivio zip, il valore predefinito è false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Ottiene/Imposta se mostrare il foglio di lavoro del grafico. Il valore predefinito è false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Ottiene/Imposta se saltare le forme invisibili nell'interfaccia utente, il valore predefinito è true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Ottiene/Imposta se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. Il valore predefinito è false. |

## Campi

| Nome | Descrizione |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Implementazione personalizzata per l'archiviazione della cache. Se desideri memorizzare la cache in modalità stream, devi impostarla e implementarla. Un host WebAssembly (IsWasm = true) deve impostarla, poiché non esiste un disco locale per la cache dei file predefinita. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Indica se utilizzare l'ID generato dal client invece dell'ID reale della forma nelle operazioni correlate alla redazione |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


