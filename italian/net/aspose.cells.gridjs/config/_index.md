---
title: "Classe Config"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.Config. Rappresenta tutte le impostazioni statiche per GridJs."
type: docs
url: /it/net/aspose.cells.gridjs/config/
---
## Config class

Rappresenta tutte le impostazioni statiche per GridJs

```csharp
public class Config
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Config](config/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Indica se adattare automaticamente la larghezza delle colonne durante il caricamento del file. Il valore predefinito è `false`. Attenzione: impostare questo a `true` eseguirà un'operazione di adattamento automatico di tutte le colonne dopo il caricamento, il che può avere un impatto notevole sulle prestazioni. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Indica se adattare automaticamente l'altezza delle righe durante il caricamento del file. Il valore predefinito è `false`. Attenzione: impostare questo a `true` eseguirà un'operazione di adattamento automatico di tutte le righe dopo il caricamento, il che può avere un impatto notevole sulle prestazioni. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Ottiene/Imposta se ottimizzare automaticamente le prestazioni di caricamento per fogli di lavoro con celle grandi. Ignorerà alcuni stili/bordi per ridurre il tempo di caricamento. Il valore predefinito è true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Ottiene/Imposta il nome del percorso base per l'URL del controller GridJs. Il valore predefinito è "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Ottiene/Imposta le PdfSaveOptions personalizzate per l'esportazione PDF. Se impostato, verrà usato al posto delle opzioni predefinite. Il valore predefinito è null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Ottiene/Imposta il numero massimo di colonne predefinito per un foglio di lavoro vuoto. Il valore predefinito è 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Ottiene/Imposta il numero massimo di righe predefinito per un foglio di lavoro vuoto. Il valore predefinito è 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Ottiene/Imposta se abilitare il rendering dei grafici lato client. Se impostato su false, GridJs tornerà a utilizzare solo immagini/forme di grafico generate dal server. Il valore predefinito è true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Ottiene/Imposta la directory della cache per memorizzare il file del foglio di calcolo. È necessario impostarla su un percorso specifico prima di utilizzare GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Ottiene/Imposta se mostrare l'intervallo massimo che include dati, stile, celle unite e forme. Se l'ultima riga o colonna contiene celle senza valore e formula ma con stile personalizzato, allora non mostreremo questa riga/colonna quando questo valore è true. Il valore predefinito è true. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Ottiene/Imposta se supportare la modifica collaborativa, il valore predefinito è false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Ottiene/Imposta se limitare il conteggio totale di forme/immagini visualizzate in un foglio di lavoro. Se impostato su true, GridJs limiterà il conteggio totale di forme o immagini visualizzate in un foglio di lavoro a MaxShapeOrImageCount. Il valore predefinito è true. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Ottiene/Imposta se GridJs viene eseguito all'interno di un host WebAssembly del browser invece di un processo server. Quando true, non viene utilizzato alcun percorso FileCacheDirectory / disco / thread di interruzione e la cache dei file deve provenire da GridJsOptions.CacheImp. GridJsOptions.IsWasm imposta questo quando il servizio GridJs viene costruito, così un unico Aspose.Cells.GridJs.dll serve entrambi gli host. Il valore predefinito è false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Ottiene/Imposta le opzioni di configurazione della cache JSON. Controlla il comportamento della cache di memoria (L1) e disco (L2) per il JSON del workbook generato. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Ottiene/Imposta se caricare solo il foglio di lavoro attivo, il valore predefinito è false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Ottiene/Imposta i secondi massimi di timeout durante il salvataggio in PDF. Il valore predefinito è 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Ottiene/Imposta il conteggio totale di forme o immagini visualizzate nel foglio attivo, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Ottiene/Imposta la larghezza o altezza massima per una forma o un'immagine; GridJs ignorerà la forma o l'immagine con larghezza o altezza superiore a questo valore, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Ottiene/Imposta il conteggio totale di forme o immagini visualizzate nella cartella di lavoro, ha effetto quando IslimitShapeOrImage=true. Il valore predefinito è 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Ottiene/Imposta le destinazioni websocket con prefisso "/topic". Il valore predefinito è "/topic/opr". Utilizzato solo in modalità collaborativa. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Ottiene/Imposta la directory della cache per le immagini. (ha effetto quando GridJsWorkbook.CacheImp è null) Il percorso predefinito sarà "_piccache" all'interno di FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Ottiene/Imposta se verificare se le immagini hanno la stessa origine, il valore predefinito è true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Ottiene/Imposta se salvare il file HTML come archivio zip, il valore predefinito è false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Ottiene/Imposta se mostrare il foglio di lavoro del grafico. Il valore predefinito è false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Ottiene/Imposta se saltare le forme invisibili nell'interfaccia utente, il valore predefinito è true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Ottiene/Imposta se utilizzare PageSetup.PrintArea per l'intervallo di visualizzazione UI quando il foglio di lavoro ha l'impostazione PageSetup per PrintArea. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Imposta la cartella dei caratteri |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Imposta le cartelle dei font |

## Campi

| Nome | Descrizione |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Indica se utilizzare l'ID generato dal client invece dell'ID reale della forma nelle operazioni correlate alla redazione |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


