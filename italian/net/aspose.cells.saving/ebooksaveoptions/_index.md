---
title: "Class EbookSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Saving.EbookSaveOptions class. Rappresenta le opzioni per salvare il file ebook."
type: docs
url: /it/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Rappresenta le opzioni per il salvataggio del file ebook.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Crea opzioni per salvare il file ebook. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Crea opzioni per salvare il file ebook. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indica se aggiungere un font generico al CSS font-family. Il valore predefinito è true(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indica se aggiungere testo tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | La directory in cui verranno salvati i file allegati. Solo per il salvataggio su stream html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio su stream html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indica se calcolare le formule prima di salvare il file html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Ottiene e imposta il prefisso del nome css, il valore predefinito è "".(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Specifica l'attributo che indica il CellName da scrivere. (ad esempio, se il valore è "id", allora per la cella "A1" l'output sarà:&lt;td id='A1'&gt;). Il valore predefinito è null.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, excel non consente di inserire una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rende la cartella di lavoro vuota dopo aver salvato il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Ottiene o imposta gli stili css aggiuntivi per il formattatore. Funziona solo quando [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) è True.  CssStyles="body { padding: 5px }";(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file html. Il valore predefinito è BackgroundColor.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Specifica il nome del font predefinito per l'esportazione html, il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale, il valore predefinito è null.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indica se vengono applicati solo stili inline, senza fare affidamento su CSS. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html, il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Ottiene o imposta il tipo di incorporamento del file font nel file html. Il valore predefinito è None, che indica che nessun font sarà incorporato nell'html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Ottimizza l'output dell'html usando proprietà CSS personalizzate. Ad esempio, nello scenario in cui ci sono più occorrenze di una stessa immagine base64, con una proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, così le prestazioni dell'html risultante possono migliorare. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indica se le entità dei caratteri html vengono sostituite con il codice decimale. (ad es. "&amp;nbsp;" è sostituito con "&amp;#160;"). Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Se non impostato, usa Encoding.UTF8 come tipo di codifica predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indica se escludere gli stili non utilizzati. Per i file html generati, escludere gli stili non utilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'html generato in seguito), impostare questa proprietà su false. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica se esportare solo il foglio di lavoro attivo in un file html. Se true, solo il foglio di lavoro attivo verrà esportato in un file html; se false, l'intera cartella di lavoro verrà esportata in un file html. Il valore predefinito è false. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Ottiene o imposta l'area di esportazione CellArea del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in html. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indica se esportare dati falsi della riga inferiore. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Rappresenta il tipo di esportazione dei commenti nei file html. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indica la regola di esportazione dei dati del file html. Il valore predefinito è All. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indica se esportare intestazioni aggiuntive quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indica se esportare le formule durante il salvataggio del file in html. Il valore predefinito è true. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indica se esportare script di frame e proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indica se esportare le linee della griglia. Il valore predefinito è false. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsoleto.**) Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica se esportare il contenuto dei fogli di lavoro nascosti. Il valore predefinito è true. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indica se esportare gli elementi anchor per gli intervalli denominati durante il salvataggio come HTML. Il valore predefinito è true. (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Ottiene o imposta l'ExportObjectListener per l'esportazione degli oggetti.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indica se esportare le intestazioni di pagina.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indica se esportare le intestazioni di pagina.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indica se esportare solo l'area di stampa in un file html. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indica se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Ottiene o imposta l'IFilePathProvider per l'esportazione del Worksheet in html separatamente.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indica se mostrare tutti i dati formattati della cella quando il contenuto supera la colonna. Se true, allora si ignora la larghezza della colonna e tutti i dati della cella verranno esportati. Se false, i dati verranno esportati come in Excel. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden"(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden"(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indica se una stringa che attraversa più celle verrà visualizzata allo stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi, per le stringhe che attraversano più celle, c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni per la creazione di grandi file html, impostando il valore su Cross, sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Specifica la versione dello standard HTML da utilizzare durante il salvataggio nel formato HTML. Il valore predefinito è HtmlVersion.Default.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indica se esportare quelle forme non visibili(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indica se i bordi della tabella sono compressi. Il valore predefinito è true.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indica se esportare i file immagine nella directory temporanea. Solo per il salvataggio in stream html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indica se esportare i commenti durante il salvataggio del file in html, il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Ottiene o imposta la modalità di layout durante il salvataggio in HTML. Il valore predefinito è Normal (Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indica il tipo di attributo target nel link `<a>`. Il valore predefinito è HtmlLinkTargetType.Parent.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in html. La dimensione del file html sarà ridotta significativamente impostando il valore su true. Il valore predefinito è false. Se si desidera importare il file html in Excel o esportare linee di griglia perfette durante il salvataggio del file in html, mantenere il valore predefinito.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indica come gli oggetti OfficeMath vengono esportati in HTML, il valore predefinito è Image.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Il titolo della pagina html. Solo per il salvataggio in stream html.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indica se i tag html (come `<div></div>`) nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se si desidera una presentazione più bella, impostare il valore su true.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indica se salvare l'html come file unico. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indica se mostrare tutti i fogli quando si salva come file html unico.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indica come gli spazi vengono visualizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è Css.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Ottiene e imposta il prefisso del nome css del tipo, come tr, col, td e così via; sono contenuti nell'elemento table che ha l'attributo specifico TableCssId. Il valore predefinito è "".(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare l'impostazione SmartArt. Il valore predefinito è false.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso.(Ereditato da [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indica se esportare la larghezza delle colonne in unità di scala in HTML. Il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false.(Ereditato da [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Crea un'istanza di EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Impostazione delle proprietà
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Salva la cartella di lavoro in un file HTML con le opzioni specificate
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


