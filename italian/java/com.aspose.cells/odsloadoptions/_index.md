---
title: "OdsLoadOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di caricamento del file ods."
type: docs
url: /it/java/com.aspose.cells/odsloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class OdsLoadOptions extends LoadOptions
```

Rappresenta le opzioni di caricamento del file ods.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OdsLoadOptions()](#OdsLoadOptions--) | Rappresenta le opzioni di caricamento del file ods. |
| [OdsLoadOptions(int type)](#OdsLoadOptions-int-) | Rappresenta le opzioni di caricamento del file ods. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getApplyExcelDefaultStyleToHyperlink()](#getApplyExcelDefaultStyleToHyperlink--) | Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale. |
| [getAutoFilter()](#getAutoFilter--) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Ottiene le opzioni dell'auto‑fitter |
| [getCheckDataValid()](#getCheckDataValid--) | Verifica se i dati sono validi nel file modello. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [getFontConfigs()](#getFontConfigs--) | Ottiene le configurazioni dei singoli caratteri. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indica se ignorare forme inutili. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Ottiene il monitor di interruzione. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [getLanguageCode()](#getLanguageCode--) | Ottiene la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [getLoadFilter()](#getLoadFilter--) | Il filtro per indicare come caricare i dati. |
| [getLoadFormat()](#getLoadFormat--) | Ottiene il formato di caricamento. |
| [getLocale()](#getLocale--) | Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata. |
| [getMemorySetting()](#getMemorySetting--) | Ottiene la modalità di memoria per la cartella di lavoro caricata. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indica se analizzare la formula durante la lettura del file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [getPassword()](#getPassword--) | Ottiene la password della cartella di lavoro. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [getRefreshPivotTables()](#getRefreshPivotTables--) | Indica se aggiornare le tabelle pivot durante il caricamento del file. |
| [getRegion()](#getRegion--) | Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata. |
| [getStandardFont()](#getStandardFont--) | Imposta il nome del carattere standard predefinito |
| [getStandardFontSize()](#getStandardFontSize--) | Imposta la dimensione del carattere standard predefinito. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hashCode()](#hashCode--) |  |
| [isClassicPivotTable()](#isClassicPivotTable--) | Indica se la tabella pivot è classica. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setApplyExcelDefaultStyleToHyperlink(boolean value)](#setApplyExcelDefaultStyleToHyperlink-boolean-) | Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Imposta le opzioni dell'auto‑fitter |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Verifica se i dati sono validi nel file modello. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClassicPivotTable(boolean value)](#setClassicPivotTable-boolean-) | Indica se la tabella pivot è classica. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Imposta le configurazioni individuali dei caratteri. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indica se ignorare forme inutili. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Imposta il monitor di interruzione. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Imposta la lingua dell'interfaccia utente della versione del Workbook in base al CountryCode che ha salvato il file. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Il filtro per indicare come caricare i dati. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Imposta la modalità di memoria per il workbook caricato. |
| [setPaperSize(int type)](#setPaperSize-int-) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indica se analizzare la formula durante la lettura del file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indica se analizzare i record memorizzati nella cache dei pivot durante il caricamento del file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Imposta la password del workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. |
| [setRefreshPivotTables(boolean value)](#setRefreshPivotTables-boolean-) | Indica se aggiornare le tabelle pivot durante il caricamento del file. |
| [setRegion(int value)](#setRegion-int-) | Imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Imposta il nome del carattere standard predefinito |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Imposta la dimensione del carattere standard predefinito. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OdsLoadOptions() {#OdsLoadOptions--}
```
public OdsLoadOptions()
```


Rappresenta le opzioni di caricamento del file ods.

### OdsLoadOptions(int type) {#OdsLoadOptions-int-}
```
public OdsLoadOptions(int type)
```


Rappresenta le opzioni di caricamento del file ods.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [LoadFormat](../../com.aspose.cells/loadformat). Il tipo di formato di caricamento. |

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
### getApplyExcelDefaultStyleToHyperlink() {#getApplyExcelDefaultStyleToHyperlink--}
```
public boolean getApplyExcelDefaultStyleToHyperlink()
```


Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale.

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
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Ottiene le configurazioni individuali dei caratteri. Funziona solo per il [Workbook](../../com.aspose.cells/workbook) che utilizza questo [LoadOptions](../../com.aspose.cells/loadoptions) per il caricamento.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Ottiene le impostazioni regionali utilizzate per la Cartella di lavoro che sarà caricata.

**Remarks**

Questa proprietà ha lo stesso effetto di [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) per impostare le impostazioni regionali.

**Returns:**
java.util.Locale
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
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

**Remarks**

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) verrà impostato allo stesso valore di questa proprietà.

**Returns:**
boolean
### getRefreshPivotTables() {#getRefreshPivotTables--}
```
public boolean getRefreshPivotTables()
```


Indica se aggiornare le tabelle pivot durante il caricamento del file.

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
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isClassicPivotTable() {#isClassicPivotTable--}
```
public boolean isClassicPivotTable()
```


Indica se la tabella pivot è classica.

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




### setApplyExcelDefaultStyleToHyperlink(boolean value) {#setApplyExcelDefaultStyleToHyperlink-boolean-}
```
public void setApplyExcelDefaultStyleToHyperlink(boolean value)
```


Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setClassicPivotTable(boolean value) {#setClassicPivotTable-boolean-}
```
public void setClassicPivotTable(boolean value)
```


Indica se la tabella pivot è classica.

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

### setRefreshPivotTables(boolean value) {#setRefreshPivotTables-boolean-}
```
public void setRefreshPivotTables(boolean value)
```


Indica se aggiornare le tabelle pivot durante il caricamento del file.

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

