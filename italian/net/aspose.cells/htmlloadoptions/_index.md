---
title: "Classe HtmlLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.HtmlLoadOptions. Rappresenta le opzioni durante l'importazione di un file HTML"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Rappresenta le opzioni durante l'importazione di un file HTML.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | Crea un'opzione per il caricamento del file. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | Crea un'opzione per il caricamento del file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) La directory in cui verranno salvati i file allegati. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Indica se adattare automaticamente colonne e righe. Il valore predefinito è false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente di inserire una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione. Se questa proprietà è false, accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato del file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. Il valore predefinito è true.(Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) se true, converte la stringa in formula quando il valore della stringa inizia con il carattere '=', il valore predefinito è false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true.(Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Indica se eliminare gli spazi ridondanti quando il testo avvolge le righe usando il tag `<br>`. Il valore predefinito è false. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Indica se rilevare formule LaTeX nel file HTML. Il valore predefinito è false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per il [`Workbook`](../workbook/) che utilizza questo [`LoadOptions`](../loadoptions/) per il caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Indica se il testo è una formula se inizia con "=\". |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Specifica come vengono caricati i collegamenti ipertestuali durante il caricamento dell'HTML. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica se ignorare forme inutili.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Il filtro per indicare come caricare i dati.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Ottiene il formato di caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Indica se importare le formule se il file HTML originale contiene formule |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la strategia per applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Specifica come gli elementi HTML &lt;p&gt; vengono renderizzati durante il caricamento dell'HTML. Il valore predefinito è Normal. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Specifica come gli elementi HTML &lt;p&gt; vengono renderizzati durante il caricamento dell'HTML. Il valore predefinito è Normal. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Ottiene e imposta la password della cartella di lavoro.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Ottiene l'ID del programma che crea il file. Solo per file MHT. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Imposta il nome del carattere standard predefinito(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Imposta la dimensione del carattere standard predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Ottiene o imposta lo StreamProviderImportHtmlFile per l'importazione di oggetti. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Indica se supportare il layout del tag `<div>` quando il file HTML lo contiene. Il valore predefinito è false. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Ottieni l'istanza di HtmlTableLoadOptionCollection |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso.(Ereditato da [`LoadOptions`](../loadoptions/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // Crea un'istanza di HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // Carica un file HTML in un Workbook usando HtmlLoadOptions
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


