---
title: "Class XmlLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.XmlLoadOptions. Rappresenta le opzioni di caricamento XML"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/
---
## XmlLoadOptions class

Rappresenta le opzioni di caricamento xml.

```csharp
public class XmlLoadOptions : LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [XmlLoadOptions](xmlloadoptions/#constructor)() | Rappresenta le opzioni di caricamento del file XML. |
| [XmlLoadOptions](xmlloadoptions/#constructor_1)(LoadFormat) | Rappresenta le opzioni di caricamento del file XML. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente di inserire una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione. Se questa proprietà è false, accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato del file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ContainsMultipleWorksheets](../../aspose.cells/xmlloadoptions/containsmultipleworksheets/) { get; set; } | Indica se importare XML come più fogli di lavoro. |
| [ConvertNumericOrDate](../../aspose.cells/xmlloadoptions/convertnumericordate/) { get; set; } | Indica se convertire il valore nel file XML in numerico o data. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [DateFormat](../../aspose.cells/xmlloadoptions/dateformat/) { get; set; } | Restituisce e imposta il formato del valore data. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro(Inherited from [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per il [`Workbook`](../workbook/) che utilizza questo [`LoadOptions`](../loadoptions/) per il caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreRootAttributes](../../aspose.cells/xmlloadoptions/ignorerootattributes/) { get; set; } | Indica se ignorare gli attributi dell'elemento radice. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica se ignorare forme inutili.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [IsXmlMap](../../aspose.cells/xmlloadoptions/isxmlmap/) { get; set; } | Indica se mappare XML in Excel. Il valore predefinito è false. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Il filtro per indicare come caricare i dati.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Ottiene il formato di caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [NumberFormat](../../aspose.cells/xmlloadoptions/numberformat/) { get; set; } | Ottiene e imposta il formato del valore numerico. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Ottiene e imposta la password della cartella di lavoro.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Imposta il nome del carattere standard predefinito(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Imposta la dimensione del carattere standard predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StartCell](../../aspose.cells/xmlloadoptions/startcell/) { get; set; } | Ottiene e imposta la cella iniziale. |
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

    public class XmlLoadOptionsDemo
    {
        public static void XmlLoadOptionsExample()
        {
            // Crea un'istanza di XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Impostazione delle proprietà
            options.StartCell = "A1";
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = "0.00";
            options.DateFormat = "yyyy-MM-dd";
            options.IgnoreRootAttributes = false;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            options.LightCellsDataHandler = null; // Assuming no data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = null; // Assuming no individual font configs are set
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = false;

            // Carica un file XML in un Workbook usando le opzioni specificate
            Workbook workbook = new Workbook("XmlLoadOptionsExample_original.xml", options);
            workbook.DefaultStyle.Font.Name = "Arial";  
            workbook.DefaultStyle.Font.Size = 10;
            
            // Salva la cartella di lavoro in un nuovo file
            workbook.Save("XmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


