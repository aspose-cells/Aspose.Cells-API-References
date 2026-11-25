---
title: "Classe DocxSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DocxSaveOptions. Rappresenta le opzioni per il salvataggio di un file .docx"
type: docs
url: /it/net/aspose.cells/docxsaveoptions/
---
## DocxSaveOptions class

Rappresenta le opzioni per il salvataggio del file .docx.

```csharp
public class DocxSaveOptions : PaginatedSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DocxSaveOptions](docxsaveoptions/#constructor)() | Rappresenta le opzioni per il salvataggio del file .docx. |
| [DocxSaveOptions](docxsaveoptions/#constructor_1)(bool) | Rappresenta le opzioni per il salvataggio del file .docx. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della dimensione della carta del pagesetup sarà ignorata, e le altre impostazioni del pagesetup continueranno ad avere effetto.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/docxsaveoptions/asflatopc/) { get; set; } | Indica se salvare come file OPC piatto che può essere generato da Open XML SDK |
| [AsNormalView](../../aspose.cells/docxsaveoptions/asnormalview/) { get; set; } | Esportazione del file Excel in file docx in visualizzazione normale. Se questa proprietà è true, verrà generata un'Area e nessuna scala avrà effetto. Il valore predefinito è false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica se verificare la compatibilità dei font per ogni carattere nel testo.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri per primi.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Ottiene o imposta le impostazioni personalizzate durante il rendering.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font di sistema predefinito per visualizzare questi caratteri Unicode.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | Indica se incorporare un file xlsx come origine dati del grafico. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Impostazione per il rendering del metafile Emf.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Ottiene o imposta il colore della griglia.(Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di linea della griglia. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere un errore nella forma, immagine, rendering del grafico, ecc. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup avranno comunque effetto. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se generare una pagina vuota quando non c'è nulla da stampare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio delle pagine. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica quali pagine non verranno stampate. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Ottiene o imposta i comportamenti di rendering specifici di Excel da applicare. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/docxsaveoptions/saveaseditableshapes/) { get; set; } | Salva tutti gli oggetti di disegno come forme modificabili nel file Word, così puoi modificarli in Word. |
| [SaveAsEditableShaps](../../aspose.cells/docxsaveoptions/saveaseditableshaps/) { get; set; } | (**Obsolete.**) Salva tutti gli oggetti di disegno come forme modificabili nel file Word. Così puoi modificarli in Word. |
| [SaveElementType](../../aspose.cells/docxsaveoptions/saveelementtype/) { get; set; } | Indica quali elementi devono essere salvati. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. (Ereditato da [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class DocxSaveOptionsDemo
    {
        public static void DocxSaveOptionsExample()
        {
            // Apri un file Excel
            Workbook workbook = new Workbook("DocxSaveOptions_original.xlsx");

            // Crea un'istanza di DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();

            // Impostazione delle proprietà
            saveOptions.DefaultFont = "MS Gothic";
            saveOptions.CheckWorkbookDefaultFont = true;
            saveOptions.CheckFontCompatibility = false;
            saveOptions.IsFontSubstitutionCharGranularity = true;
            saveOptions.OnePagePerSheet = true;
            saveOptions.AllColumnsInOnePagePerSheet = false;
            saveOptions.IgnoreError = true;
            saveOptions.OutputBlankPageWhenNothingToPrint = false;
            saveOptions.PageIndex = 0;  // Starting page index (0-based index)
            saveOptions.PageCount = 2;  // Number of pages to be printed
            saveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            saveOptions.GridlineType = GridlineType.Dotted;
            saveOptions.TextCrossType = TextCrossType.CrossKeep;
            saveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            saveOptions.SheetSet = SheetSet.All;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = @"C:\Cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = false;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Salva il documento in formato DOCX
            workbook.Save("DocxSaveOptionsExample.docx", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


