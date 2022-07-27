---
title: LoadOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni di caricamento del file.
type: docs
weight: 4000
url: /it/net/aspose.cells/loadoptions/
---
## LoadOptions class

Rappresenta le opzioni di caricamento del file.

```csharp
public class LoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Crea un'opzione per caricare il file. |
| [LoadOptions](loadoptions#constructor_1)(LoadFormat) | Crea un'opzione per caricare il file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Verifica se i dati sono validi nel file modello. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Indica se controllare la restrizione del file excel quando l'utente modifica gli oggetti correlati alle celle. Ad esempio, excel non consente l'immissione di un valore di stringa più lungo di 32K. Quando si immette un valore più lungo di 32K, ad esempio da Cell.PutValue(string), se questo è true, otterrai un'eccezione. Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che later tu possa restituire il valore della stringa completo per altri formati di file come CSV. Tuttavia, se hai impostato un tale tipo di valore che non è valido per il formato di file excel, non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Ottiene o imposta le informazioni sulle impostazioni cultura del sistema al momento del caricamento del file. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il[`Workbook`](../workbook) che usa questo[`LoadOptions`](../loadoptions) caricare.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Ottiene e imposta il monitor di interruzione. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro in base a CountryCode che ha salvato il file. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Il filtro per indicare come caricare i dati. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Ottiene il formato di caricamento. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Ottiene o imposta le opzioni di utilizzo della memoria. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indica se analizzare la formula durante la lettura del file. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indica se l'analisi dei record memorizzati nella cache del pivot durante il caricamento del file. Il valore predefinito è false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Ottiene e imposta la password della cartella di lavoro. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Imposta il formato carta di stampa predefinito dall'impostazione predefinita della stampante. |

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
