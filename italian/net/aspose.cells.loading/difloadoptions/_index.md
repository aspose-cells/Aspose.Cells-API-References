---
title: "Classe DifLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "**Aspose.Cells.Loading.DifLoadOptions** classe. Rappresenta le opzioni di caricamento del file .dif"
type: docs
url: /it/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Rappresenta le opzioni di caricamento del file .dif.

```csharp
public class DifLoadOptions : LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Le opzioni. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. (Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Ottiene e imposta le opzioni dell'adattatore automatico (Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello. (Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite **Cell.PutValue(string)**, se questa proprietà è true, verrà generata un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa in altri formati di file come CSV. Tuttavia, se hai impostato un valore non valido per il formato file Excel, non dovresti salvare la cartella di lavoro in formato Excel successivamente. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. (Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che verrà caricata.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il [`Workbook`](../../aspose.cells/workbook/) che utilizza questo [`LoadOptions`](../../aspose.cells/loadoptions/) per il caricamento.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica se ignorare forme inutili.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata da un file modello. Il valore predefinito è true.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Il filtro per indicare come caricare i dati.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Ottiene il formato di caricamento.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Ottiene o imposta la modalità di memoria per la Cartella di lavoro caricata.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati della tabella pivot durante il caricamento del file. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Ottiene e imposta la password della Cartella di lavoro.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che verrà caricata.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Imposta il nome del carattere standard predefinito(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Imposta la dimensione del carattere standard predefinita.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita.(Ereditato da [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea un'istanza di DifLoadOptions
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Crea una cartella di lavoro (usando il costruttore senza parametri)
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Calcola le formule, se presenti
            workbook.CalculateFormula();

            // Salva la cartella di lavoro in formato DIF
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Ora dimostra il caricamento del file DIF con DifLoadOptions
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Carica il file DIF salvato con le opzioni
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Accedi ai dati della cartella di lavoro caricata
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Salva i dati caricati in XLSX per verifica
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


