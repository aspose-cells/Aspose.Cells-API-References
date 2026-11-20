---
title: "TxtLoadOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per il caricamento di file di testo."
type: docs
url: /it/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Rappresenta le opzioni per il caricamento di file di testo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Crea le opzioni per il caricamento di file di testo. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Crea le opzioni per il caricamento di file di testo. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Ottiene le opzioni dell'auto‑fitter |
| [getCheckDataValid()](#getCheckDataValid--) | Verifica se i dati sono validi nel file modello. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. |
| [getConvertNumericData()](#getConvertNumericData--) | Restituisce un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [getEncoding()](#getEncoding--) | Ottiene la codifica predefinita. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Indica se estende i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. |
| [getFontConfigs()](#getFontConfigs--) | Ottiene le configurazioni dei singoli caratteri. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | Il conteggio delle colonne di intestazione da ripetere per i fogli estesi. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | Il conteggio delle righe di intestazione da ripetere per i fogli estesi. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indica se ignorare forme inutili. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Ottiene il monitor di interruzione. |
| [getKeepPrecision()](#getKeepPrecision--) | Indica se non analizzare un valore stringa quando la lunghezza è 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [getLanguageCode()](#getLanguageCode--) | Ottiene la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [getLoadFilter()](#getLoadFilter--) | Il filtro per indicare come caricare i dati. |
| [getLoadFormat()](#getLoadFormat--) | Ottiene il formato di caricamento. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indica la strategia da applicare allo stile per i valori analizzati quando si converte un valore stringa in numero o data/ora. |
| [getLocale()](#getLocale--) | Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata. |
| [getMaxColumnCount()](#getMaxColumnCount--) | Il conteggio massimo di colonne da importare per un foglio. |
| [getMaxRowCount()](#getMaxRowCount--) | Il numero massimo di righe da importare per un foglio. |
| [getMemorySetting()](#getMemorySetting--) | Ottiene la modalità di memoria per la cartella di lavoro caricata. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica se analizzare la formula durante la lettura del file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [getPassword()](#getPassword--) | Ottiene la password della cartella di lavoro. |
| [getPreferredParsers()](#getPreferredParsers--) | Ottiene i parser di valore preferiti per il caricamento del file di testo. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [getRegion()](#getRegion--) | Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata. |
| [getSeparator()](#getSeparator--) | Ottiene il separatore di caratteri del file di testo. |
| [getSeparatorString()](#getSeparatorString--) | Ottiene un valore stringa come separatore. |
| [getStandardFont()](#getStandardFont--) | Imposta il nome del carattere standard predefinito |
| [getStandardFontSize()](#getStandardFontSize--) | Imposta la dimensione del carattere standard predefinito. |
| [getTextQualifier()](#getTextQualifier--) | Specifica il qualificatore di testo per i valori delle celle. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Indica se i delimitatori consecutivi devono essere trattati come uno solo. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hasFormula()](#hasFormula--) | Indica se il testo è una formula se inizia con "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Indica se esiste un qualificatore di testo per il valore della cella. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True indica che il file contiene diverse codifiche. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Imposta le opzioni dell'auto‑fitter |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Verifica se i dati sono validi nel file modello. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Imposta la codifica predefinita. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Indica se estende i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Imposta le configurazioni individuali dei caratteri. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indica se il testo è una formula se inizia con "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Indica se esiste un qualificatore di testo per il valore della cella. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | Il conteggio delle colonne di intestazione da ripetere per i fogli estesi. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | Il conteggio delle righe di intestazione da ripetere per i fogli estesi. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indica se ignorare forme inutili. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Imposta il monitor di interruzione. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indica se non analizzare un valore stringa quando la lunghezza è 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Imposta la lingua dell'interfaccia utente della versione del Workbook in base al CountryCode che ha salvato il file. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Il filtro per indicare come caricare i dati. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Indica la strategia da applicare allo stile per i valori analizzati quando si converte un valore stringa in numero o data/ora. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | Il conteggio massimo di colonne da importare per un foglio. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | Il numero massimo di righe da importare per un foglio. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Imposta la modalità di memoria per il workbook caricato. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True indica che il file contiene diverse codifiche. |
| [setPaperSize(int type)](#setPaperSize-int-) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica se analizzare la formula durante la lettura del file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Imposta la password del workbook. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Imposta i parser di valore preferiti per il caricamento del file di testo. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [setRegion(int value)](#setRegion-int-) | Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato. |
| [setSeparator(char value)](#setSeparator-char-) | Imposta il separatore di caratteri del file di testo. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Imposta un valore stringa come separatore. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Imposta il nome del carattere standard predefinito |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Imposta la dimensione del carattere standard predefinito. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Specifica il qualificatore di testo per i valori delle celle. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Indica se i delimitatori consecutivi devono essere trattati come uno solo. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Crea le opzioni per il caricamento di file di testo.

**Remarks**

Il tipo di file di caricamento predefinito è CSV.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Crea le opzioni per il caricamento di file di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Il formato di caricamento |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indica se filtrare automaticamente i dati durante il caricamento dei file.

**Remarks**

A volte, sebbene l'autofiltro sia impostato, le righe corrispondenti non sono nascoste nel file. Ora funziona solo per i file SpreadSheetML.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Ottiene le opzioni dell'auto‑fitter

**Remarks**

Solo per file xlsx, spreadsheetML al momento.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Verifica se i dati sono validi nel file modello.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è invalido per il formato file Excel, non dovresti salvare il workbook in formato Excel successivamente. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Ottiene un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. Il valore predefinito è true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ottiene un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ottiene la codifica predefinita. Si applica solo ai file csv.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false.

**Remarks**

Se questa proprietà è true, i dati aggiuntivi saranno inseriti nel foglio successivo dietro quello corrente (se il foglio corrente è l'ultimo, un nuovo foglio sarà aggiunto alla cartella di lavoro corrente). Se questa proprietà è false, i dati che superano il limite saranno ignorati.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Ottiene le configurazioni individuali dei caratteri. Funziona solo per il [Workbook](../../com.aspose.cells/workbook) che utilizza questo [LoadOptions](../../com.aspose.cells/loadoptions) per il caricamento.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


Il conteggio delle colonne di intestazione da ripetere per i fogli estesi.

**Remarks**

Le colonne di intestazione specificate da questa proprietà saranno duplicate per i fogli estesi. Questa proprietà ha effetto solo quando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) è true.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


Il conteggio delle righe di intestazione da ripetere per i fogli estesi.

**Remarks**

Le righe di intestazione specificate da questa proprietà saranno duplicate per i fogli estesi. Questa proprietà ha effetto solo quando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) è true.

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignora i dati che non vengono stampati se si stampa direttamente il file

**Remarks**

Solo per file xlsx.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Indica se ignorare forme inutili.

**Remarks**

Funziona solo per file xlsx, xlsb e xlsm. Ci sono molte forme identiche sovrapposte che sono inutili in alcuni file; possiamo ignorarle durante il caricamento dei file.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Ottiene il monitor di interruzione.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indica se non analizzare un valore stringa quando la lunghezza è 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true.

**Remarks**

Per scenari in cui l'utente deve solo leggere alcuni contenuti dal file modello e non necessita di salvare nuovamente il workbook, impostare questa proprietà su false può migliorare le prestazioni, soprattutto se usata insieme a qualche tipo di LoadFilter,

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Ottiene la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Il filtro per indicare come caricare i dati.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Ottiene il formato di caricamento.

Vedi [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Indica la strategia da applicare allo stile per i valori analizzati quando si converte un valore stringa in numero o data/ora.

Vedi [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.

**Remarks**

Questa proprietà ha lo stesso effetto di [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) per impostare le impostazioni regionali.

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


Il conteggio massimo di colonne da importare per un foglio.

**Remarks**

Le colonne che superano questo limite saranno ignorate o estese al foglio successivo in base a [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Questo conteggio include le colonne di intestazione([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Il valore massimo è il limite di colonne del formato file corrispondente, ad esempio per i file xlsx è 16384. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà utilizzato anche il limite massimo.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


Il numero massimo di righe da importare per un foglio.

**Remarks**

Le righe che superano questo limite saranno ignorate o estese al foglio successivo in base a [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Questo conteggio include le righe di intestazione([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Il valore massimo consentito è il limite di righe del formato file corrispondente, ad esempio per i file xlsx è 1048576. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà utilizzato anche il limite massimo.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Ottiene la modalità di memoria per la cartella di lavoro caricata.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Per ulteriori dettagli sulla modalità di memoria, consulta [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indica se analizzare la formula durante la lettura del file.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm e Xlsm perché le formule nei file sono memorizzate come stringa di formula.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indica se analizzare i record cache dei pivot durante il caricamento del file. Il valore predefinito è false.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm, Xlsm e xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Ottiene la password della cartella di lavoro.

**Returns:**
java.lang.String
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Ottiene i parser di valore preferiti per il caricamento del file di testo.

**Remarks**

parsers[0] è il parser che verrà utilizzato per la prima colonna nel file modello di testo, parsers[1] è il parser che verrà utilizzato per la seconda colonna, ...etc. L'ultimo (parsers[parsers.length-1]) sarà usato per tutte le altre colonne a partire da parsers.length-1. Se un elemento è null, la colonna corrispondente sarà analizzata dal parser predefinito di Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) verrà impostato allo stesso valore di questa proprietà.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Le impostazioni regionali possono essere utilizzate per inizializzare alcune funzionalità della cartella di lavoro, come i caratteri, i temi e così via. Per i formati di file basati su testo, come CSV, HTML, ..., le impostazioni regionali verranno inoltre utilizzate per rilevare i formati numerici e analizzare i valori di testo in valori numerici o data/ora per le celle. Questa impostazione verrà mantenuta per la cartella di lavoro istanziata in seguito, cioè, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) della cartella di lavoro utilizzerà la stessa regione di questa proprietà.

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Ottiene il separatore di caratteri del file di testo.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ottiene un valore stringa come separatore.

**Returns:**
java.lang.String
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Imposta il nome del carattere standard predefinito

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Imposta la dimensione del carattere standard predefinito.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'.

**Remarks**

Quando si imposta questa proprietà, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) diventerà true automaticamente.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Indica se i delimitatori consecutivi devono essere trattati come uno solo.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale sarà rimosso dal valore della cella corrispondente e [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) sarà impostato su true per la cella.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indica se il testo è una formula se inizia con "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True indica che il file contiene diverse codifiche.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indica se filtrare automaticamente i dati durante il caricamento dei file.

**Remarks**

A volte, sebbene l'autofiltro sia impostato, le righe corrispondenti non sono nascoste nel file. Ora funziona solo per i file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Imposta le opzioni dell'auto‑fitter

**Remarks**

Solo per file xlsx, spreadsheetML al momento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Verifica se i dati sono validi nel file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è invalido per il formato file Excel, non dovresti salvare il workbook in formato Excel successivamente. Altrimenti potrebbero verificarsi errori inattesi nel file Excel generato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Imposta la codifica predefinita. Si applica solo ai file csv.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false.

**Remarks**

Se questa proprietà è true, i dati aggiuntivi saranno inseriti nel foglio successivo dietro quello corrente (se il foglio corrente è l'ultimo, un nuovo foglio sarà aggiunto alla cartella di lavoro corrente). Se questa proprietà è false, i dati che superano il limite saranno ignorati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Imposta configurazioni di carattere individuali. Funziona solo per la [Workbook](../../com.aspose.cells/workbook) che utilizza queste [LoadOptions](../../com.aspose.cells/loadoptions) per il caricamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indica se il testo è una formula se inizia con "=".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


Il conteggio delle colonne di intestazione da ripetere per i fogli estesi.

**Remarks**

Le colonne di intestazione specificate da questa proprietà saranno duplicate per i fogli estesi. Questa proprietà ha effetto solo quando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


Il conteggio delle righe di intestazione da ripetere per i fogli estesi.

**Remarks**

Le righe di intestazione specificate da questa proprietà saranno duplicate per i fogli estesi. Questa proprietà ha effetto solo quando [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignora i dati che non vengono stampati se si stampa direttamente il file

**Remarks**

Solo per file xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Indica se ignorare forme inutili.

**Remarks**

Funziona solo per file xlsx, xlsb e xlsm. Ci sono molte forme identiche sovrapposte che sono inutili in alcuni file; possiamo ignorarle durante il caricamento dei file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Imposta il monitor di interruzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indica se non analizzare un valore stringa quando la lunghezza è 15.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true.

**Remarks**

Per scenari in cui l'utente deve solo leggere alcuni contenuti dal file modello e non necessita di salvare nuovamente il workbook, impostare questa proprietà su false può migliorare le prestazioni, soprattutto se usata insieme a qualche tipo di LoadFilter,

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Imposta la lingua dell'interfaccia utente della versione del Workbook in base al CountryCode che ha salvato il file.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Il filtro per indicare come caricare i dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Indica la strategia da applicare allo stile per i valori analizzati quando si converte un valore stringa in numero o data/ora.

Vedi [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato.

**Remarks**

Questa proprietà ha lo stesso effetto di [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) per impostare le impostazioni regionali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


Il conteggio massimo di colonne da importare per un foglio.

**Remarks**

Le colonne che superano questo limite saranno ignorate o estese al foglio successivo in base a [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Questo conteggio include le colonne di intestazione([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Il valore massimo è il limite di colonne del formato file corrispondente, ad esempio per i file xlsx è 16384. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà utilizzato anche il limite massimo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


Il numero massimo di righe da importare per un foglio.

**Remarks**

Le righe che superano questo limite saranno ignorate o estese al foglio successivo in base a [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Questo conteggio include le righe di intestazione([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Il valore massimo consentito è il limite di righe del formato file corrispondente, ad esempio per i file xlsx è 1048576. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà utilizzato anche il limite massimo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Imposta la modalità di memoria per il workbook caricato.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Per ulteriori dettagli sulla modalità di memoria, consulta [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True indica che il file contiene diverse codifiche.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita.

**Remarks**

Se non esiste un'impostazione relativa alle dimensioni della carta, MS Excel utilizzerà l'impostazione predefinita della stampante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). La dimensione della carta predefinita. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indica se analizzare la formula durante la lettura del file.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm e Xlsm perché le formule nei file sono memorizzate come stringa di formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indica se analizzare i record cache dei pivot durante il caricamento del file. Il valore predefinito è false.

**Remarks**

Si applica solo ai file Excel Xlsx, Xltx, Xltm, Xlsm e xlsb.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Imposta la password del workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Imposta i parser di valore preferiti per il caricamento del file di testo.

**Remarks**

parsers[0] è il parser che verrà utilizzato per la prima colonna nel file modello di testo, parsers[1] è il parser che verrà utilizzato per la seconda colonna, ...etc. L'ultimo (parsers[parsers.length-1]) sarà usato per tutte le altre colonne a partire da parsers.length-1. Se un elemento è null, la colonna corrispondente sarà analizzata dal parser predefinito di Aspose.Cells.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) verrà impostato allo stesso valore di questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Le impostazioni regionali possono essere utilizzate per inizializzare alcune funzionalità della cartella di lavoro, come i caratteri, i temi e così via. Per i formati di file basati su testo, come CSV, HTML, ..., le impostazioni regionali verranno inoltre utilizzate per rilevare i formati numerici e analizzare i valori di testo in valori numerici o data/ora per le celle. Questa impostazione verrà mantenuta per la cartella di lavoro istanziata in seguito, cioè, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) della cartella di lavoro utilizzerà la stessa regione di questa proprietà.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Imposta il separatore di caratteri del file di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Imposta un valore stringa come separatore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Imposta il nome del carattere standard predefinito

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Imposta la dimensione del carattere standard predefinito.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'.

**Remarks**

Quando si imposta questa proprietà, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) diventerà true automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Indica se i delimitatori consecutivi devono essere trattati come uno solo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale sarà rimosso dal valore della cella corrispondente e [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) sarà impostato su true per la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Imposta la callback di avviso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

