---
title: "Classe GridHtmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions. Rappresenta le opzioni per il salvataggio di file html"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Rappresenta le opzioni per salvare il file HTML.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Crea le opzioni per salvare il file html. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Crea le opzioni per salvare il file htm. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream html. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio in stream html. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | La cartella dei file nella cache è usata per memorizzare alcuni dati di grandi dimensioni.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Rendi la cartella di lavoro vuota dopo aver salvato il file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Specifica il nome del font predefinito per l'esportazione html, il font predefinito verrà utilizzato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale, il valore predefinito è null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica se esportare l'intera cartella di lavoro in un file html. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Ottiene o imposta l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata quando si salva il file in html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Indica se esportare le intestazioni quando si salva il file in html. Il valore predefinito è false. Se vuoi importare il file html in Excel, mantieni il valore predefinito. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Indica se esportare solo l'area di stampa nel file html. Il valore predefinito è false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Indica se esportare la singola scheda quando il file ha solo un foglio di lavoro. Il valore predefinito è false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Indica se esportare i commenti durante il salvataggio del file in HTML, il valore predefinito è false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | Il titolo della pagina HTML. Solo per il salvataggio in stream HTML. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Analizza il tag html nella cella, come valore della cella o come tag html, il valore predefinito è true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Indica se aggiornare i dati della cache del grafico (Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file.(Ereditato da [`GridSaveOptions`](../gridsaveoptions/).) |

### Vedi anche

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


