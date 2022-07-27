---
title: TxtLoadOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni per il caricamento del file di testo.
type: docs
weight: 6110
url: /it/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Rappresenta le opzioni per il caricamento del file di testo.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | Crea le opzioni per il caricamento del file di testo. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | Crea le opzioni per il caricamento del file di testo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Ottiene e imposta le opzioni di adattamento automatico |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Verifica se i dati sono validi nel file modello. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Indica se controllare la restrizione del file excel quando l'utente modifica gli oggetti correlati alle celle. Ad esempio, excel non consente l'immissione di un valore di stringa più lungo di 32K. Quando si immette un valore più lungo di 32K, ad esempio da Cell.PutValue(string), se questo è true, otterrai un'eccezione. Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che later tu possa restituire il valore della stringa completo per altri formati di file come CSV. Tuttavia, se hai impostato un tale tipo di valore che non è valido per il formato di file excel, non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Ottiene o imposta le informazioni sulle impostazioni cultura del sistema al momento del caricamento del file. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo al file CSV. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | Se estende i dati al foglio successivo quando le righe o le colonne di dati superano il limite. Se questa proprietà è vera, i dati extra verranno estesi al foglio successivo dietro a quello corrente (se il foglio corrente è l'ultimo, verrà aggiunto un nuovo foglio alla cartella di lavoro corrente). Se questa proprietà è falsa, i dati che superano il limite verranno ignorati. L'impostazione predefinita è false; |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il[`Workbook`](../workbook) che usa questo[`LoadOptions`](../loadoptions) caricare.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | Indica se il testo è formula se inizia con "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | Se esiste un qualificatore di testo per il valore della cella. L'impostazione predefinita è true. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Ottiene e imposta il monitor di interruzione. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | True significa che il file contiene diverse codifiche. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro in base a CountryCode che ha salvato il file. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Il filtro per indicare come caricare i dati. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Ottiene il formato di caricamento. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indica la strategia per applicare lo stile per i valori analizzati durante la conversione del valore della stringa in numero o data/ora. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Ottiene o imposta le opzioni di utilizzo della memoria. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indica se analizzare la formula durante la lettura del file. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indica se l'analisi dei record memorizzati nella cache del pivot durante il caricamento del file. Il valore predefinito è false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Ottiene e imposta la password della cartella di lavoro. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | Ottiene e imposta i parser di valori preferiti per il caricamento del file di testo. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | Ottiene e imposta il separatore di caratteri del file di testo. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | Ottiene e imposta un valore stringa come separatore. |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | Se i delimitatori consecutivi devono essere trattati come uno. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | Indica se il segno di virgoletta singola iniziale deve essere preso come parte del valore di una cella. L'impostazione predefinita è true. Se è falso, la virgoletta singola iniziale verrà rimossa dal valore della cella corrispondente e[`QuotePrefix`](../style/quoteprefix) sarà impostato come true per la cella. |
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
