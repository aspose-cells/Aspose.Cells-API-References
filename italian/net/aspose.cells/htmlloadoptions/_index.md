---
title: HtmlLoadOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni durante limportazione di un file html.
type: docs
weight: 3730
url: /it/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Rappresenta le opzioni durante l'importazione di un file html.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions#constructor)() | Crea un'opzione per caricare il file. |
| [HtmlLoadOptions](htmlloadoptions#constructor_1)(LoadFormat) | Crea un'opzione per caricare il file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows) { get; set; } | Indica se si adattano automaticamente colonne e righe. Il valore predefinito è false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Verifica se i dati sono validi nel file modello. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Indica se controllare la restrizione del file excel quando l'utente modifica gli oggetti correlati alle celle. Ad esempio, excel non consente l'immissione di un valore di stringa più lungo di 32K. Quando si immette un valore più lungo di 32K, ad esempio da Cell.PutValue(string), se questo è true, otterrai un'eccezione. Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che later tu possa restituire il valore della stringa completo per altri formati di file come CSV. Tuttavia, se hai impostato un tale tipo di valore che non è valido per il formato di file excel, non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata) { get; set; } | se true, converte la stringa in formula quando il valore della stringa inizia con il carattere '=', il valore predefinito è false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Ottiene o imposta le informazioni sulle impostazioni cultura del sistema al momento del caricamento del file. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces) { get; set; } | Indica se eliminare gli spazi ridondanti quando il testo va a capo delle righe utilizzando il tag &lt;br&gt;. Il valore predefinito è false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo al file CSV. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il[`Workbook`](../workbook) che usa questo[`LoadOptions`](../loadoptions) caricare.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Ottiene e imposta il monitor di interruzione. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro in base a CountryCode che ha salvato il file. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Il filtro per indicare come caricare i dati. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Ottiene il formato di caricamento. |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas) { get; set; } | Indica se si stanno importando formule se il file html originale contiene formule |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indica la strategia per applicare lo stile per i valori analizzati durante la conversione del valore della stringa in numero o data/ora. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Ottiene o imposta le opzioni di utilizzo della memoria. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indica se analizzare la formula durante la lettura del file. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indica se l'analisi dei record memorizzati nella cache del pivot durante il caricamento del file. Il valore predefinito è false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Ottiene e imposta la password della cartella di lavoro. |
| [ProgId](../../aspose.cells/htmlloadoptions/progid) { get; } | Ottiene l'id del programma di creazione del file. Solo per file MHT. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file. |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider) { get; set; } | Ottiene o imposta StreamProviderImportHtmlFile per l'importazione di oggetti. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag) { get; set; } | Indica se supporta il layout del tag &lt;div&gt; quando il file html contiene tag &lt;div&gt;. Il valore predefinito è false. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Imposta il formato carta di stampa predefinito dall'impostazione predefinita della stampante. |

### Guarda anche

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
