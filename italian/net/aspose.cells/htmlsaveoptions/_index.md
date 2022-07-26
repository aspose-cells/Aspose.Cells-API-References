---
title: HtmlSaveOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni per il salvataggio del file html.
type: docs
weight: 3740
url: /it/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Rappresenta le opzioni per il salvataggio del file html.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Crea opzioni per il salvataggio del file html. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Crea opzioni per salvare il file htm. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Indica se aggiungere il testo della descrizione comando quando i dati non possono essere visualizzati completamente. Il valore predefinito è false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | La directory in cui verranno salvati i file allegati. Solo per il salvataggio nel flusso html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Specifica il prefisso Url dei file allegati come l'immagine nel file html. Solo per il salvataggio nel flusso html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La cartella dei file nella cache viene utilizzata per memorizzare dati di grandi dimensioni. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Ottiene e imposta il prefisso del nome css, il valore predefinito è "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Rendi vuota la cartella di lavoro dopo aver salvato il file. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Specificare il nome del carattere predefinito per l'esportazione html, il carattere predefinito verrà utilizzato quando il carattere dello stile non è esistente, Se questa proprietà è nulla, Aspose.Cells utilizzerà il carattere universale che ha la stessa famiglia del carattere originale, il valore predefinito è null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Indica se disabilita i commenti condizionali rivelati di livello inferiore durante l'esportazione del file in html, il valore predefinito è false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Se non impostato, usa Encoding.UTF8 come tipo di codifica predefinito. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Indica se esclude gli stili non utilizzati. Per i file html generati, l'esclusione degli stili non utilizzati può ridurre le dimensioni del file senza influire sugli effetti visivi. Quindi il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (come lo scenario in cui l'utente ha bisogno di ripristinare la cartella di lavoro dall'html generato in un secondo momento), impostare questa proprietà su false . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indica se si sta esportando l'intera cartella di lavoro in un file html. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Ottiene o imposta la CellArea di esportazione del foglio di lavoro attivo corrente. Se si imposta questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata quando si salva il file in html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Indica se esportare dati della riga inferiore fasulli. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Indica se esportare le coordinate excel di celle non vuote durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare l'html di output in Excel, mantieni il valore predefinito. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Indica la regola di esportazione dei dati del file html. Il valore predefinito è All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht per eccellere, mantieni il valore predefinito. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Indica se esportare intestazioni extra quando la lunghezza del testo è maggiore della colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Indica se esportare la formula durante il salvataggio del file in html. Il valore predefinito è true. Se desideri importare l'html di output in Excel, mantieni il valore predefinito. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Indica se esportare script frame e proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Indica se si sta esportando il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Indica se esportare intestazioni di pagina. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Indica se esportare intestazioni di pagina. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Indica se si esporta solo l'area di stampa su file html. Il valore predefinito è false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Indica se esporta le intestazioni di riga e colonna del foglio durante il salvataggio in file HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Indica se esportare lo stile del bordo simile quando lo stile del bordo non è supportato dai browser. Se desideri importare il file html o mht in excel, mantieni il valore predefinito. Il valore predefinito è false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Indica se esportare la scheda singola quando il file ha un solo foglio di lavoro. Il valore predefinito è false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Indica se esportare il foglio di lavoro CSS separatamente. Il valore predefinito è false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Ottiene o imposta l'IFilePathProvider per esportare il foglio di lavoro in html separatamente. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Colonna nascosta (la larghezza di questa colonna è 0) in excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è "Rimuovi", la colonna nascosta non verrebbe emessa, se il valore è "Nascosto", la colonna verrebbe stato emesso, ma era nascosto, il valore predefinito è "Nascosto" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Riga nascosta (l'altezza di questa riga è 0) in excel, prima di salvarla in formato html, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrebbe emessa, se il valore è "Nascosto", la riga verrebbe stato emesso, ma era nascosto, il valore predefinito è "Nascosto" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Indica se una stringa tra celle verrà visualizzata allo stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Predefinito, quindi, per le stringhe tra celle, c'è poca differenza tra l'html file creati da Aspose.Cells e MS Excel. Ma le prestazioni per la creazione di file html di grandi dimensioni, impostando il valore su Cross sarebbero molte volte più veloci rispetto a impostarlo su Default o Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Indica se esportare quelle forme non visibili |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Ottieni l'oggetto ImageOrPrintOptions prima di esportare |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Indica se si utilizza l'unità scalabile per descrivere la larghezza dell'immagine quando si utilizza l'unità scalabile per descrivere la larghezza della colonna. Il valore predefinito è true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Indica se esportare i file di immagine nella directory temporanea. Solo per il salvataggio nel flusso html. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Indica se si esportano commenti durante il salvataggio del file in html, il valore predefinito è false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Indica se si utilizza il collegamento del percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | Indicando il tipo di attributo di destinazione nel collegamento &lt;a&gt;, il valore predefinito è HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica se unire le aree di formattazione condizionale e validazione prima di salvare il file. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Indica se si unisce forzatamente un elemento TD vuoto durante l'esportazione del file in html. La dimensione del file html verrà notevolmente ridotta dopo aver impostato il valore su true. Il valore predefinito è falso. Se desideri importare il file html in Excel o esportare linee di griglia perfette quando salvi il file in html, mantieni il valore predefinito. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Il titolo della pagina html. Solo per il salvataggio nel flusso html. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Analizza il tag html nella cella, come ,come valore della cella,o come tag html,il valore predefinito è true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false.se vuoi ottenere una presentazione più bella , imposta il valore su true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica se aggiornare i dati della cache del grafico |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Indica se salvare l'html come file singolo. Il valore predefinito è false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Ottiene il formato del file di salvataggio. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Indica se mostrare tutti i fogli quando si salva come un unico file html. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Ottiene o imposta IStreamProvider per l'esportazione di oggetti. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Ottiene e imposta il prefisso del tipo css name come tr,col,td e così via, sono contenuti nell'elemento della tabella che ha l'attributo TableCssId specifico. Il valore predefinito è "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Indica se si utilizza l'unità scalabile per descrivere la larghezza della colonna durante l'esportazione del file in html. Il valore predefinito è false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Indica se si esegue lo zoom avanti o indietro dell'html tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in html, il valore predefinito è false. |

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
