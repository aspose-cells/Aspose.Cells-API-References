---
title: "Classe PaginatedSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.PaginatedSaveOptions. Rappresenta le opzioni per l'impaginazione"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/
---
## PaginatedSaveOptions class

Rappresenta le opzioni per l'impaginazione.

```csharp
public abstract class PaginatedSaveOptions : SaveOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza del formato carta di pagesetup verrà ignorata, mentre le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica se verificare la compatibilità del carattere per ogni carattere nel testo. |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per visualizzare prima questi caratteri. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Impostazione per il rendering del metafile Emf. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Ottiene o imposta il colore della griglia. |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di griglia. |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere relativo a forme, immagini, rendering di grafici, ecc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. Il formato carta di pagesetup sarà invalido, ma le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su 0 della prima pagina da salvare. |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica quali pagine non saranno stampate. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Ottiene o imposta i comportamenti di rendering specifici di Excel da applicare. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
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

    public class PaginatedSaveOptionsDemo
    {
        public static void PaginatedSaveOptionsExample()
        {
            // Apri un file Excel
            Workbook workbook = new Workbook("PaginatedSaveOptionsExample_original.xlsx");

            // Crea un'istanza di PaginatedSaveOptions
            PdfSaveOptions options = new PdfSaveOptions();

            // Impostazione delle proprietà
            options.DefaultFont = "Arial";
            options.CheckWorkbookDefaultFont = true;
            options.CheckFontCompatibility = true;
            options.IsFontSubstitutionCharGranularity = true;
            options.OnePagePerSheet = false;
            options.AllColumnsInOnePagePerSheet = false;
            options.IgnoreError = true;
            options.OutputBlankPageWhenNothingToPrint = false;
            options.PageIndex = 3; // Starting page index (0-based index)
            options.PageCount = 2; // Number of pages to be printed
            options.PrintingPageType = PrintingPageType.IgnoreBlank;
            options.GridlineType = GridlineType.Dotted;
            options.TextCrossType = TextCrossType.CrossKeep;
            options.DefaultEditLanguage = DefaultEditLanguage.English;
            options.SheetSet = new SheetSet(new int[] { workbook.Worksheets.ActiveSheetIndex });
            options.ClearData = false;
            options.CachedFileFolder = "C:\\Temp";
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // Salva il file PDF
            workbook.Save("PaginatedSaveOptionsExample.pdf", options);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


