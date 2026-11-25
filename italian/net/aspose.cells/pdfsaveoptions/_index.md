---
title: "Classe PdfSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.PdfSaveOptions. Rappresenta le opzioni per il salvataggio di un file pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Rappresenta le opzioni per il salvataggio di un file PDF.

```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Crea le opzioni per il salvataggio di un file pdf. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della dimensione della carta del pagesetup sarà ignorata, e le altre impostazioni del pagesetup continueranno ad avere effetto.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Ottiene e imposta l'oggetto [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Indica se calcolare le formule prima di salvare il file pdf. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica se verificare la compatibilità dei font per ogni carattere nel testo.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri per primi.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Ottiene o imposta il livello di conformità agli standard PDF per i documenti di output. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Ottiene o imposta l'ora di generazione del documento pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Ottiene o imposta un valore che determina il modo in cui [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) vengono esportati in un file PDF. Il valore predefinito è None. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Ottiene o imposta le impostazioni personalizzate durante il rendering.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font di sistema predefinito per visualizzare questi caratteri Unicode.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Indica se incorporare gli allegati per gli oggetti Ole in Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True per incorporare i caratteri TrueType. Influisce solo sui caratteri ASCII 32-127. I caratteri per codici superiori a 127 sono sempre incorporati. I caratteri sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b. Il valore predefinito è true. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Impostazione per il rendering del metafile Emf.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Indica se esportare la struttura del documento. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Ottiene o imposta la codifica dei caratteri incorporati nel pdf. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Ottiene o imposta il colore della griglia.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di linea della griglia. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere un errore nella forma, immagine, rendering del grafico, ecc. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Obsolete.**) Rappresenta il tipo di immagine durante la conversione del grafico e della forma. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup avranno comunque effetto. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Ottiene e imposta il tipo di ottimizzazione pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se generare una pagina vuota quando non c'è nulla da stampare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio delle pagine. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Indica l'algoritmo di compressione |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica quali pagine non verranno stampate. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Ottiene o imposta il produttore del documento pdf generato. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Ottiene o imposta i comportamenti di rendering specifici di Excel da applicare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Ottiene o imposta la filigrana in output. |
| [ZoomBehavior](../../aspose.cells/pdfsaveoptions/zoombehavior/) { get; set; } | Ottiene o imposta la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. Il valore predefinito è None. |
| [ZoomFactor](../../aspose.cells/pdfsaveoptions/zoomfactor/) { get; set; } | Ottiene o imposta la percentuale di zoom utilizzata quando [`ZoomBehavior`](./zoombehavior/) è ZoomFactor. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Imposta il PPI desiderato (pixel per pollice) per il ridimensionamento delle immagini e la qualità JPEG. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata, e le immagini che superano il PPI specificato (pixel per pollice) saranno ridimensionate. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;
    using System.Drawing;

    public class PdfSaveOptionsDemo
    {
        public static void PdfSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");

            // Crea un'istanza di PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Imposta varie proprietà
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = "Aspose.Cells";
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = "Arial";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = "C:\\Temp";
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Imposta le opzioni di sicurezza
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = "OwnerPassword",
                UserPassword = "UserPassword",
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Imposta la filigrana
            RenderingFont font = new RenderingFont("Calibri", 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Salva la cartella di lavoro come file PDF
            workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


