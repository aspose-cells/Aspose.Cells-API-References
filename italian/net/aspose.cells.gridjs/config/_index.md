---
title: Config
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta tutte le impostazioni per GridJs
type: docs
weight: 10
url: /it/net/aspose.cells.gridjs/config/
---
## Config class

Rappresenta tutte le impostazioni per GridJs

```csharp
public class Config
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Config](config)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells) { get; set; } |  |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol) { get; set; } | Imposta/Ottiene la colonna massima predefinita per un foglio di lavoro vuoto |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow) { get; set; } | Imposta la riga massima predefinita per un foglio di lavoro vuoto |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory) { get; set; } | Imposta/Ottiene la directory della cache per il file della cartella di lavoro |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent) { get; set; } | Imposta se mostrare l'intervallo massimo che include dati, stile, celle e forme unite. il valore predefinito è true .se l'ultima riga o colonna contiene celle senza valore e formula ma ha uno stile personalizzato , non lo mostreremo riga/colonna quando questo valore è true |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage) { get; set; } | Imposta se limitare la forma totale di visualizzazione/conteggio di immagini all'interno di un foglio di lavoro, se impostato su true, GridJs limiterà la forma di visualizzazione totale/dimensione dell'immagine all'interno di un foglio di lavoro a MaxShapeOrImageCount il valore predefinito è true |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds) { get; set; } | Imposta /Ottiene il tempo massimo di secondi scaduti quando salva in pdf |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount) { get; set; } | Imposta /Ottiene la forma di visualizzazione totale/il conteggio delle immagini all'interno del foglio attivo, ci vorrà affec quando IslimitShapes=true |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight) { get; set; } | Imposta /Ottiene la larghezza o l'altezza massima per una forma/immagine,GridJs ignorerà la forma/immagine con la larghezza o l'altezza maggiore di questa, ci vorrà affec quando IslimitShapes=true |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount) { get; set; } | Imposta /Ottiene la forma di visualizzazione totale/il conteggio delle immagini all'interno dell'intera cartella di lavoro, ci vorrà affec quando IslimitShapes=true |
| static [PageSize](../../aspose.cells.gridjs/config/pagesize) { get; set; } | Imposta se eseguire l'impaginazione GridJs limiterà la dimensione della riga in base a PageSize, se PageSize è -1, non eseguirà l'impaginazione il valore predefinito è -1 |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory) { get; set; } | Imposta/Ottiene la directory della cache per le immagini |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting) { get; set; } | Imposta se controllare se l'immagine ha la stessa origine, il valore predefinito è true il valore predefinito è true |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip) { get; set; } | Imposta se salvare il file html come archivio zip, il valore predefinito è false il valore predefinito è true |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder)(string, bool) | Imposta la cartella dei caratteri |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders)(string[], bool) | Imposta le cartelle dei caratteri |

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* assemblea [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
