---
title: "Classe AbstractTextLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractTextLoadOptions. Opzioni comuni per il caricamento di valori di testo"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/
---
## AbstractTextLoadOptions class

Opzioni comuni per il caricamento dei valori di testo

```csharp
public class AbstractTextLoadOptions : LoadOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente di inserire una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio con Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione. Se questa proprietà è false, accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato del file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. Il valore predefinito è true. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per il [`Workbook`](../workbook/) che utilizza questo [`LoadOptions`](../loadoptions/) per il caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indica se ignorare forme inutili.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Il filtro per indicare come caricare i dati.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Ottiene il formato di caricamento.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indica la strategia da applicare allo stile per i valori analizzati quando si converte una stringa in numero o data/ora. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Ottiene e imposta la password della cartella di lavoro.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsoleto.**) Imposta il nome del carattere standard predefinito(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsoleto.**) Imposta la dimensione del carattere standard predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso.(Ereditato da [`LoadOptions`](../loadoptions/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita.(Ereditato da [`LoadOptions`](../loadoptions/).) |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Text;

namespace AsposeCellsExamples
{
    // Implementazione personalizzata di AbstractTextLoadOptions
    public class CustomTextLoadOptions : AbstractTextLoadOptions
    {
        public CustomTextLoadOptions()
        {
            // Imposta la codifica predefinita su UTF8
            this.Encoding = Encoding.UTF8;

            // Imposta LoadStyleStrategy su None
            this.LoadStyleStrategy = TxtLoadStyleStrategy.None;

            // Abilita la conversione dei dati numerici
            this.ConvertNumericData = true;

            // Abilita la conversione dei dati di data
            this.ConvertDateTimeData = true;

            // Mantieni la precisione per le stringhe con lunghezza 15
            this.KeepPrecision = true;
        }
    }

    public class TextLoadOptionsDemo
    {
        public static void RunDemo()
        {
            // Crea un'istanza di CustomTextLoadOptions
            CustomTextLoadOptions loadOptions = new CustomTextLoadOptions();

            // Carica un file CSV con le opzioni di caricamento personalizzate
            Workbook workbook = new Workbook("TextLoadOptionsDemo_original.csv", loadOptions);

            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];

            // Stampa il valore della prima cella
            Console.WriteLine(sheet.Cells["A1"].StringValue);

            // Salva la cartella di lavoro in un nuovo file
            workbook.Save("TextLoadOptionsDemo.xlsx");
            workbook.Save("TextLoadOptionsDemo.pdf");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


