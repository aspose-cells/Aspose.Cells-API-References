---
title: "Classe HtmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.HtmlSaveOptions class. Rappresenta le opzioni per salvare il file html"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Rappresenta le opzioni per salvare il file HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Crea le opzioni per salvare il file html. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Crea le opzioni per salvare il file htm. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indica se aggiungere un font generico al CSS font-family. Il valore predefinito è true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio in stream html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indica se calcolare le formule prima di salvare il file html. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Ottiene e imposta il prefisso del nome css, il valore predefinito è "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Specifica l'attributo che indica il CellName da scrivere. (ad esempio, se il valore è "id", allora per la cella "A1" l'output sarà:&lt;td id='A1'&gt;). Il valore predefinito è null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Ottiene o imposta gli stili css aggiuntivi per il formattatore. Funziona solo quando [`SaveAsSingleFile`](./saveassinglefile/) è True.  CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file html. Il valore predefinito è BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Specifica il nome del font predefinito per l'esportazione html, il font predefinito verrà utilizzato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale, il valore predefinito è null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indica se vengono applicati solo gli stili inline, senza fare affidamento su CSS. Il valore predefinito è false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html, il valore predefinito è false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Ottiene o imposta il tipo di incorporamento del file font nel file html. Il valore predefinito è None, il che indica che nessun font sarà incorporato nell'html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Ottimizza l'output dell'html utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze di una stessa immagine base64, con una proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, migliorando così le prestazioni dell'html risultante. Il valore predefinito è false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indica se le entità dei caratteri html vengono sostituite con il codice decimale. (ad esempio, "&amp;nbsp;" è sostituito con "&amp;#160;"). Il valore predefinito è false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indica se escludere gli stili non utilizzati. Per i file html generati, escludere gli stili non utilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'html generato in seguito), impostare questa proprietà su false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indica se esportare solo il foglio di lavoro attivo in un file html. Se true, solo il foglio di lavoro attivo sarà esportato in un file html; se false, l'intera cartella di lavoro sarà esportata in un file html. Il valore predefinito è false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Ottiene o imposta l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata sarà esportata durante il salvataggio del file in html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indica se esportare dati falsi della riga inferiore. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indica se esportare le coordinate Excel delle celle non vuote quando si salva il file in html. Il valore predefinito è false. Se vuoi importare l'html di output in Excel, mantieni il valore predefinito. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Rappresenta il tipo di esportazione dei commenti nei file html. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indica la regola di esportazione dei dati del file html. Il valore predefinito è All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se vuoi importare il file html in Excel, mantieni il valore predefinito. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indica se esportare le formule quando si salva il file in html. Il valore predefinito è true. Se vuoi importare l'html di output in Excel, mantieni il valore predefinito. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indica se esportare gli script del frame e le proprietà del documento. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Indica se esportare le intestazioni di righe e colonne del foglio quando si salva in file HTML. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indica se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indica se esportare gli elementi anchor per gli intervalli denominati quando si salva come HTML. Il valore predefinito è true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Ottiene o imposta l'ExportObjectListener per l'esportazione degli oggetti. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indica se esportare le intestazioni di pagina. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indica se esportare le intestazioni di pagina. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indica se esportare solo l'area di stampa nel file html. Il valore predefinito è false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indica se esportare le intestazioni di righe e colonne del foglio quando si salva in file HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. Il valore predefinito è false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indica se esportare la singola scheda quando il file ha solo un foglio di lavoro. Il valore predefinito è false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indica se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Ottiene o imposta l'IFilePathProvider per l'esportazione del Worksheet in html separatamente. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indica se mostrare tutti i dati formattati della cella quando supera la larghezza della colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella verranno esportati. Se false, i dati verranno esportati come in Excel. Il valore predefinito è false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è \"Remove\", la colonna nascosta non verrà emessa; se il valore è \"Hidden\", la colonna verrà emessa ma rimarrà nascosta. Il valore predefinito è \"Hidden\". |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa, se il valore è "Hidden", la riga verrà emessa, ma sarà nascosta, il valore predefinito è "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato HTML. Per impostazione predefinita il valore è Default, quindi, per le stringhe che attraversano più celle, c'è poca differenza tra i file HTML creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni per la creazione di file HTML di grandi dimensioni, impostando il valore su Cross, sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Specifica la versione dello standard HTML da utilizzare quando si salva il formato HTML. Il valore predefinito è HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indica se esportare le forme non visibili |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indica se i bordi della tabella sono compressi. Il valore predefinito è true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio in stream HTML. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indica se esportare i commenti durante il salvataggio del file in HTML, il valore predefinito è false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Ottiene o imposta la modalità di layout quando si salva in HTML. Il valore predefinito è Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indica il tipo di attributo target nel link `<a>`. Il valore predefinito è HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in HTML. La dimensione del file HTML sarà ridotta significativamente impostando il valore su true. Il valore predefinito è false. Se desideri importare il file HTML in Excel o esportare linee di griglia perfette quando salvi il file in HTML, mantieni il valore predefinito. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indica come gli oggetti OfficeMath vengono esportati in HTML, il valore predefinito è Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Il titolo della pagina HTML. Solo per il salvataggio in stream HTML. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indica se i tag HTML (come `<div></div>`) nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indica se il file HTML o MHT è la preferenza di presentazione. Il valore predefinito è false. Se desideri ottenere una presentazione più bella, imposta il valore su true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indica se salvare l'HTML come file unico. Il valore predefinito è false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indica se mostrare tutti i fogli quando si salva come file HTML unico. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indica come gli spazi vengono renderizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Ottiene e imposta il prefisso del nome CSS di tipo, come tr, col, td e così via; sono contenuti nell'elemento table che possiede l'attributo specifico TableCssId. Il valore predefinito è \"\". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indica se esportare la larghezza delle colonne in unità di scala in HTML. Il valore predefinito è false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea un'istanza di HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Salva la cartella di lavoro come HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


