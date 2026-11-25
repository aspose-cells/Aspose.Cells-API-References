---
title: "Classe TxtLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.TxtLoadOptions. Rappresenta le opzioni per il caricamento di un file di testo"
type: docs
url: /it/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Rappresenta le opzioni per il caricamento di file di testo.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Crea le opzioni per il caricamento di un file di testo. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Crea le opzioni per il caricamento di un file di testo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente di inserire una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione. Se questa proprietà è false, accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato del file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. Il valore predefinito è true.(Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true.(Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per il [`Workbook`](../workbook/) che utilizza questo [`LoadOptions`](../loadoptions/) per il caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Indica se il testo è una formula se inizia con "=\". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Indica se è presente un qualificatore di testo per il valore della cella. Il valore predefinito è true. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | Il conteggio delle colonne di intestazione da ripetere per i fogli estesi. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | Il conteggio delle righe di intestazione da ripetere per i fogli estesi. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica se ignorare forme inutili.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | True indica che il file contiene diverse codifiche. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Il filtro per indicare come caricare i dati.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Ottiene il formato di caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la strategia per applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora. (Ereditato da [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | Il conteggio massimo di colonne da importare per un foglio. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | Il conteggio massimo di righe da importare per un foglio. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Ottiene e imposta la password della cartella di lavoro.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Ottiene e imposta i parser di valore preferiti per il caricamento di un file di testo. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Ottiene e imposta il separatore di caratteri del file di testo. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Ottiene e imposta un valore stringa come separatore. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Imposta il nome del carattere standard predefinito(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Imposta la dimensione del carattere standard predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Indica se i delimitatori consecutivi devono essere trattati come uno. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e [`QuotePrefix`](../style/quoteprefix/) verrà impostato su true per la cella. |
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
    using System.Text;

    public class TxtLoadOptionsDemo
    {
        public static void TxtLoadOptionsExample()
        {
            // Crea un'istanza di TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                SeparatorString = ",",
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = '\"',
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = "password",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Carica un file CSV con le opzioni specificate
            Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("TxtLoadOptionsExample.xlsx");

            return;
        }
    }

    // Implementazioni fittizie per classi/interfacce di riferimento
    public class InterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested => false;
    }

    public class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine(warningInfo.Description);
        }
    }

    public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet) => true;
        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


