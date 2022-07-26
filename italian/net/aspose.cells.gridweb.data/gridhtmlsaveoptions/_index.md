---
title: GridHtmlSaveOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni per il salvataggio del file html.
type: docs
weight: 250
url: /it/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Rappresenta le opzioni per il salvataggio del file html.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Crea opzioni per il salvataggio del file html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Crea opzioni per salvare il file htm. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | La directory in cui verranno salvati i file allegati. Solo per il salvataggio nel flusso html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Specifica il prefisso Url dei file allegati come l'immagine nel file html. Solo per il salvataggio nel flusso html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | La cartella dei file nella cache viene utilizzata per memorizzare dati di grandi dimensioni. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Rendi vuota la cartella di lavoro dopo aver salvato il file. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Specificare il nome del carattere predefinito per l'esportazione html, il carattere predefinito verrà utilizzato quando il carattere dello stile non è esistente, Se questa proprietà è nulla, Aspose.Cells utilizzerà il carattere universale che ha la stessa famiglia del carattere originale, il valore predefinito è null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Se non impostato, usa Encoding.UTF8 come tipo di codifica predefinito. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indica se si sta esportando l'intera cartella di lavoro in un file html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Ottiene o imposta la CellArea di esportazione del foglio di lavoro attivo corrente. Se si imposta questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata quando si salva il file in html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Indica se esportare le intestazioni durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Indica se si sta esportando il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Indica se si esporta solo l'area di stampa su file html. Il valore predefinito è false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Indica se esportare la scheda singola quando il file ha un solo foglio di lavoro. Il valore predefinito è false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Indica se si esportano commenti durante il salvataggio del file in html, il valore predefinito è false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Indica se si utilizza il collegamento del percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Indica se unire le aree di formattazione condizionale e validazione prima di salvare il file. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Il titolo della pagina html. Solo per il salvataggio nel flusso html. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Analizza il tag html nella cella, come ,come valore della cella,o come tag html,il valore predefinito è true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false.se vuoi ottenere una presentazione più bella , imposta il valore su true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Indica se aggiornare i dati della cache del grafico |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Ottiene il formato del file di salvataggio. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. |

### Guarda anche

* class [GridSaveOptions](../gridsaveoptions)
* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
