---
title: "WorkbookSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le impostazioni della cartella di lavoro."
type: docs
url: /it/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Rappresenta tutte le impostazioni della cartella di lavoro.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [dispose()](#dispose--) | Rilascia risorse. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Ottiene l'autore del file. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro. |
| [getAutoRecover()](#getAutoRecover--) | Indica se il file è contrassegnato per il ripristino automatico. |
| [getBuildVersion()](#getBuildVersion--) | Specifica la versione incrementale pubblica dell'applicazione. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Specifica la versione OOXML per il documento di output. |
| [getCrashSave()](#getCrashSave--) | Indica se l'applicazione ha salvato l'ultima volta il file della cartella di lavoro dopo un arresto anomalo. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Indica se l'applicazione ha aperto l'ultima volta la cartella di lavoro per il recupero dei dati. |
| [getDate1904()](#getDate1904--) | Ottiene un valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Ottiene la risoluzione predefinita dell'immagine. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Ottiene le impostazioni per i valori predefiniti delle proprietà relative allo stile per questa cartella di lavoro. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Indica se scartare i dati immagine modificati. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Indica se e come visualizzare gli oggetti nella cartella di lavoro. |
| [getEnableMacros()](#getEnableMacros--) | Abilita macro; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Ottiene la prima scheda del foglio di lavoro visibile. |
| [getFormulaSettings()](#getFormulaSettings--) | Ottiene le impostazioni per le funzionalità relative alle formule. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Ottiene le impostazioni di globalizzazione. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Ottiene se nascondere l'elenco dei campi per la tabella pivot. |
| [getLanguageCode()](#getLanguageCode--) | Ottiene la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [getLocale()](#getLocale--) | Ottiene la localizzazione utilizzata da questa cartella di lavoro. |
| [getMaxColumn()](#getMaxColumn--) | Ottiene l'indice massimo della colonna, basato su zero. |
| [getMaxRow()](#getMaxRow--) | Ottiene l'indice massimo della riga, basato su zero. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Ottiene il numero massimo di riga della formula condivisa. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Ottiene la limitazione degli elementi unici per campo |
| [getMemorySetting()](#getMemorySetting--) | Ottiene le opzioni di utilizzo della memoria. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Ottiene il separatore decimale per la formattazione/analisi dei valori numerici. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Ottiene il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. |
| [getPaperSize()](#getPaperSize--) | Ottiene la dimensione predefinita della carta di stampa. |
| [getPassword()](#getPassword--) | Rappresenta la password di crittografia del file Workbook. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento. |
| [getProtectionType()](#getProtectionType--) | Ottiene il tipo di protezione del workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Indica se impostare la proprietà [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella |
| [getRegion()](#getRegion--) | Ottiene le impostazioni regionali per il workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Vero se le informazioni personali possono essere rimosse dal workbook specificato. |
| [getRepairLoad()](#getRepairLoad--) | Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione. |
| [getResourceProvider()](#getResourceProvider--) | Ottiene il provider di stream per risorse esterne, ad esempio il caricamento dei dati immagine per un'immagine di tipo "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Ottiene come l'applicazione visualizza le forme in questo workbook |
| [getShared()](#getShared--) | Ottiene un valore che indica se il Workbook è condiviso. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [getShowTabs()](#getShowTabs--) | Ottiene un valore che indica se le schede del Workbook sono visualizzate. |
| [getSignificantDigits()](#getSignificantDigits--) | Ottiene il numero di cifre significative. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Ottiene il tipo di cifre significative per l'emissione dei valori numerici in questo workbook. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Ottiene le opzioni del tag intelligente. |
| [getStreamProvider()](#getStreamProvider--) | Ottiene il provider di stream per risorse esterne. |
| [getThemeFont(int type)](#getThemeFont-int-) | Ottiene il nome del carattere predefinito del tema. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Indica se aggiornare il bordo delle celle adiacenti. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Ottiene come vengono aggiornati i collegamenti esterni quando il workbook viene aperto. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [getWindowHeight()](#getWindowHeight--) | L'altezza della finestra, in unità di punto. |
| [getWindowHeightCM()](#getWindowHeightCM--) | L'altezza della finestra, in unità di centimetro. |
| [getWindowHeightInch()](#getWindowHeightInch--) | L'altezza della finestra, in unità di pollice. |
| [getWindowLeft()](#getWindowLeft--) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto. |
| [getWindowLeftCM()](#getWindowLeftCM--) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. |
| [getWindowLeftInch()](#getWindowLeftInch--) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. |
| [getWindowTop()](#getWindowTop--) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto. |
| [getWindowTopCM()](#getWindowTopCM--) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro. |
| [getWindowTopInch()](#getWindowTopInch--) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice. |
| [getWindowWidth()](#getWindowWidth--) | La larghezza della finestra, in unità di punto. |
| [getWindowWidthCM()](#getWindowWidthCM--) | La larghezza della finestra, in unità di centimetro. |
| [getWindowWidthInch()](#getWindowWidthInch--) | La larghezza della finestra, in unità di pollice. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indica se essere compatibile con WPS. |
| [getWriteProtection()](#getWriteProtection--) | Fornisce l'accesso alle opzioni di protezione in scrittura della cartella di lavoro. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Indica se crittografare la cartella di lavoro con la password predefinita se la struttura e le finestre della cartella di lavoro sono bloccate. |
| [isEncrypted()](#isEncrypted--) | Restituisce un valore che indica se è richiesta una password per aprire questa cartella di lavoro. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Restituisce un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale. |
| [isHidden()](#isHidden--) | Indica se questa cartella di lavoro è nascosta. |
| [isMinimized()](#isMinimized--) | Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona. |
| [isProtected()](#isProtected--) | Restituisce un valore che indica se la struttura o la finestra della cartella di lavoro è protetta. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Restituisce un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Imposta l'autore del file. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Indica se il file è contrassegnato per il ripristino automatico. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Specifica la versione incrementale pubblica dell'applicazione. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setCompliance(int value)](#setCompliance-int-) | Specifica la versione OOXML per il documento di output. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Indica se l'applicazione ha salvato l'ultima volta il file della cartella di lavoro dopo un arresto anomalo. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Indica se l'applicazione ha aperto l'ultima volta la cartella di lavoro per il recupero dei dati. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Imposta un valore che rappresenta se la cartella di lavoro utilizza il sistema di data 1904. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Indica se crittografare la cartella di lavoro con la password predefinita se la struttura e le finestre della cartella di lavoro sono bloccate. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Imposta la risoluzione predefinita dell'immagine. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Indica se scartare i dati immagine modificati. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Indica se e come visualizzare gli oggetti nella cartella di lavoro. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Abilita macro; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Imposta la scheda del foglio di lavoro visibile per prima. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Imposta le impostazioni di globalizzazione. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se questa cartella di lavoro è nascosta. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Imposta se nascondere l'elenco dei campi per la tabella pivot. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Imposta la lingua dell'interfaccia utente della versione del Workbook in base al CountryCode che ha salvato il file. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Imposta la localizzazione utilizzata da questa cartella di lavoro. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Imposta il numero massimo di righe della formula condivisa. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Imposta il limite di elementi unici per campo |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Imposta le opzioni di utilizzo della memoria. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Imposta il separatore decimale per la formattazione/analisi dei valori numerici. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro. |
| [setPaperSize(int value)](#setPaperSize-int-) | Imposta la dimensione predefinita della carta di stampa. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Rappresenta la password di crittografia del file Workbook. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Indica se impostare la proprietà [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella |
| [setRegion(int value)](#setRegion-int-) | Imposta le impostazioni regionali per la cartella di lavoro. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Vero se le informazioni personali possono essere rimosse dal workbook specificato. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Imposta il provider di flusso per risorse esterne, ad esempio il caricamento dei dati immagine per un'immagine di tipo "LinkToFile". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Imposta come l'applicazione visualizza le forme in questa cartella di lavoro |
| [setShared(boolean value)](#setShared-boolean-) | Imposta un valore che indica se la cartella di lavoro è condivisa. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Imposta un valore che indica se le schede della cartella di lavoro sono visualizzate. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Imposta il numero di cifre significative. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Imposta il tipo di cifre significative per l'emissione dei valori numerici in questa cartella di lavoro. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Imposta il provider di flusso per risorse esterne. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Indica se aggiornare il bordo delle celle adiacenti. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Imposta come aggiornare i collegamenti esterni quando la cartella di lavoro viene aperta. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | L'altezza della finestra, in unità di punto. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | L'altezza della finestra, in unità di centimetro. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | L'altezza della finestra, in unità di pollice. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. |
| [setWindowTop(double value)](#setWindowTop-double-) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | La larghezza della finestra, in unità di punto. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | La larghezza della finestra, in unità di centimetro. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | La larghezza della finestra, in unità di pollice. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indica se essere compatibile con WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Rilascia risorse.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ottiene l'autore del file.

**Remarks**

Non è impostato, controlla prima [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) poi controlla l'utente dell'Environment.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Indica se il file è contrassegnato per il ripristino automatico.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Specifica la versione incrementale pubblica dell'applicazione.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro.

**Remarks**

Il valore predefinito è true. Solo per file Excel97-2003 xls o xlt.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376\_2006.

Vedi [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Solo per file .xlsx.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Indica se l'applicazione ha salvato l'ultima volta il file della cartella di lavoro dopo un arresto anomalo.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Indica se l'applicazione ha aperto l'ultima volta la cartella di lavoro per il recupero dei dati.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Ottiene un valore che indica se la cartella di lavoro utilizza il sistema di data 1904.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Ottiene la risoluzione predefinita dell'immagine.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Ottiene le impostazioni per i valori predefiniti delle proprietà relative allo stile per questa cartella di lavoro.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Indica se scartare i dati immagine modificati.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Indica se e come visualizzare gli oggetti nella cartella di lavoro.

Vedi [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Abilita macro;

**Remarks**

Ora funziona solo quando si copia un foglio di lavoro in un altro foglio di lavoro all'interno di una cartella di lavoro.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Ottiene la prima scheda del foglio di lavoro visibile.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Ottiene le impostazioni per le funzionalità relative alle formule.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Ottiene le impostazioni di globalizzazione.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Ottiene se nascondere l'elenco dei campi per la tabella pivot.

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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Ottiene la localizzazione utilizzata da questa cartella di lavoro.

**Remarks**

Restituisce null se né la Localizzazione né [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) sono impostati.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Ottiene l'indice massimo della colonna, basato su zero.

**Remarks**

Restituisce 255 se il formato file è Excel97-2003;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Ottiene l'indice massimo della riga, basato su zero.

**Remarks**

Restituisce 65535 se il formato file è Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Ottiene il numero massimo di riga della formula condivisa.

**Remarks**

Se il numero è troppo grande, l'autofiltro funziona molto lentamente in MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Ottiene la limitazione degli elementi unici per campo

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Ottiene le opzioni di utilizzo della memoria. La nuova opzione sarà presa come opzione predefinita per i fogli di lavoro appena creati ma non avrà effetto sui fogli di lavoro esistenti.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Per ulteriori dettagli sulla modalità di memoria, consulta [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Ottiene il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della Regione corrente.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Ottiene il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della Regione corrente.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Ottiene la dimensione predefinita della carta di stampa.

Vedi [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Se non esiste un'impostazione relativa alle dimensioni della carta, MS Excel utilizzerà l'impostazione predefinita della stampante.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Rappresenta la password di crittografia del file Workbook.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Ottiene il tipo di protezione del workbook.

Vedi [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Indica se impostare la proprietà [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Ottiene le impostazioni regionali per il workbook.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Impostazioni regionali utilizzate dal componente Aspose.Cells per una cartella di lavoro caricata da un file modello: i). Per un file XLS, esistono campi definiti per le impostazioni regionali e MS Excel salva i dati delle impostazioni regionali nel file durante il salvataggio del file XLS. Pertanto, utilizziamo la regione salvata nel file modello per la cartella di lavoro. Se non si desidera utilizzare la regione salvata nel file XLS, si prega di reimpostarla a quella prevista (ad esempio, CountryCode.Default) dopo aver caricato il file modello. Inoltre, salviamo anche il valore specificato dall'utente (tramite questo metodo) nel file quando si salva un file XLS. ii). Per altri formati di file, come XLSX, XLSB... ecc., non è definito alcun campo per le impostazioni regionali nella specifica del formato file. Pertanto, utilizziamo le impostazioni regionali dell'ambiente dell'applicazione per la cartella di lavoro. E il valore specificato dall'utente (tramite questo metodo) non può essere conservato per i file generati con tali formati. 2. Per l'effetto di visualizzazione in MS Excel: le impostazioni regionali applicate qui possono avere effetto solo a runtime con il componente Aspose.Cells e non quando si visualizza il file generato con MS Excel. Anche per il file XLS generato in cui i dati delle impostazioni regionali specificate sono stati salvati, quando lo si visualizza/modifica con MS Excel, la regione utilizzata da MS Excel per eseguire la formattazione è sempre quella predefinita dell'ambiente in cui MS Excel è in esecuzione, non quella salvata nel file. È un comportamento di MS Excel e non può essere modificato tramite codice.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Vero se le informazioni personali possono essere rimosse dal workbook specificato.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Ottiene il provider di stream per risorse esterne, ad esempio il caricamento dei dati immagine per un'immagine di tipo "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Ottiene come l'applicazione visualizza le forme in questo workbook

Vedi [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Ottiene un valore che indica se il Workbook è condiviso.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Ottiene un valore che indica se le schede del Workbook sono visualizzate.

**Remarks**

Il valore predefinito è true.

**Example**

Il codice seguente nasconde le schede dei fogli e i pulsanti di scorrimento delle schede per il foglio di calcolo.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Ottiene il numero di cifre significative. Il valore predefinito è [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Può essere solo 15 o 17 al momento. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Questa proprietà sarà rimossa 12 mesi dopo a partire da giugno 2025. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Ottiene il tipo di cifre significative per l'emissione di valori numerici in questa cartella di lavoro. Il valore predefinito è [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Vedi [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Ottiene le opzioni del tag intelligente.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ottiene il provider di stream per risorse esterne.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ResourceProvider. Questa proprietà sarà rimossa 12 mesi dopo a partire da giugno 2022. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Ottiene il nome del carattere predefinito del tema.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Il tipo di schema del carattere. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Indica se aggiornare il bordo delle celle adiacenti.

**Remarks**

Il valore predefinito è false. Per esempio: il bordo inferiore della cella A1 è aggiornato, il bordo superiore della cella A2 dovrebbe essere modificato anch'esso.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Ottiene come vengono aggiornati i collegamenti esterni quando il workbook viene aperto.

Vedi [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


L'altezza della finestra, in unità di punto.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


L'altezza della finestra, in unità di centimetro.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


L'altezza della finestra, in unità di pollice.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetri.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollici.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


La larghezza della finestra, in unità di punto.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


La larghezza della finestra, in unità di centimetro.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


La larghezza della finestra, in unità di pollice.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indica se essere compatibile con WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Fornisce l'accesso alle opzioni di protezione in scrittura della cartella di lavoro.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Indica se crittografare la cartella di lavoro con la password predefinita se la struttura e le finestre della cartella di lavoro sono bloccate.

**Remarks**

Il valore predefinito è ora false. È lo stesso di MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Restituisce un valore che indica se è richiesta una password per aprire questa cartella di lavoro.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Restituisce un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale.

**Remarks**

Il valore predefinito è true.

**Example**

Il codice seguente rende invisibile la barra di scorrimento orizzontale per il foglio di calcolo.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica se questa cartella di lavoro è nascosta.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Restituisce un valore che indica se la struttura o la finestra della cartella di lavoro è protetta.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Restituisce un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale.

**Remarks**

Il valore predefinito è true.

**Example**

Il codice seguente rende invisibile la barra di scorrimento verticale per il foglio di calcolo.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Imposta l'autore del file.

**Remarks**

Non è impostato, controlla prima [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) poi controlla l'utente dell'Environment.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Indica se il file è contrassegnato per il ripristino automatico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Specifica la versione incrementale pubblica dell'applicazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro.

**Remarks**

Il valore predefinito è true. Solo per file Excel97-2003 xls o xlt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376\_2006.

Vedi [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Solo per file .xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Indica se l'applicazione ha salvato l'ultima volta il file della cartella di lavoro dopo un arresto anomalo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Indica se l'applicazione ha aperto l'ultima volta la cartella di lavoro per il recupero dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Imposta un valore che rappresenta se la cartella di lavoro utilizza il sistema di data 1904.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Indica se crittografare la cartella di lavoro con la password predefinita se la struttura e le finestre della cartella di lavoro sono bloccate.

**Remarks**

Il valore predefinito è ora false. È lo stesso di MS Excel 2013.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Imposta la risoluzione predefinita dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Indica se scartare i dati immagine modificati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Indica se e come visualizzare gli oggetti nella cartella di lavoro.

Vedi [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Abilita macro;

**Remarks**

Ora funziona solo quando si copia un foglio di lavoro in un altro foglio di lavoro all'interno di una cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Imposta la scheda del foglio di lavoro visibile per prima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Imposta le impostazioni di globalizzazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica se questa cartella di lavoro è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Imposta se nascondere l'elenco dei campi per la tabella pivot.

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

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Imposta la localizzazione utilizzata da questa cartella di lavoro.

**Remarks**

Restituisce null se né la Localizzazione né [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) sono impostati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Imposta il numero massimo di righe della formula condivisa.

**Remarks**

Se il numero è troppo grande, l'autofiltro funziona molto lentamente in MS Excel 2013.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Imposta il limite di elementi unici per campo

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Imposta le opzioni di utilizzo della memoria. La nuova opzione verrà presa come opzione predefinita per i fogli di lavoro appena creati, ma non avrà effetto sui fogli di lavoro esistenti.

Vedi [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Per ulteriori dettagli sulla modalità di memoria, consulta [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della regione corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Il tipo di orientamento della pagina |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Imposta la dimensione predefinita della carta di stampa.

Vedi [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Se non esiste un'impostazione relativa alle dimensioni della carta, MS Excel utilizzerà l'impostazione predefinita della stampante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Rappresenta la password di crittografia del file Workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Indica se impostare la proprietà [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Imposta le impostazioni regionali per la cartella di lavoro.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Impostazioni regionali utilizzate dal componente Aspose.Cells per una cartella di lavoro caricata da un file modello: i). Per un file XLS, esistono campi definiti per le impostazioni regionali e MS Excel salva i dati delle impostazioni regionali nel file durante il salvataggio del file XLS. Pertanto, utilizziamo la regione salvata nel file modello per la cartella di lavoro. Se non si desidera utilizzare la regione salvata nel file XLS, si prega di reimpostarla a quella prevista (ad esempio, CountryCode.Default) dopo aver caricato il file modello. Inoltre, salviamo anche il valore specificato dall'utente (tramite questo metodo) nel file quando si salva un file XLS. ii). Per altri formati di file, come XLSX, XLSB... ecc., non è definito alcun campo per le impostazioni regionali nella specifica del formato file. Pertanto, utilizziamo le impostazioni regionali dell'ambiente dell'applicazione per la cartella di lavoro. E il valore specificato dall'utente (tramite questo metodo) non può essere conservato per i file generati con tali formati. 2. Per l'effetto di visualizzazione in MS Excel: le impostazioni regionali applicate qui possono avere effetto solo a runtime con il componente Aspose.Cells e non quando si visualizza il file generato con MS Excel. Anche per il file XLS generato in cui i dati delle impostazioni regionali specificate sono stati salvati, quando lo si visualizza/modifica con MS Excel, la regione utilizzata da MS Excel per eseguire la formattazione è sempre quella predefinita dell'ambiente in cui MS Excel è in esecuzione, non quella salvata nel file. È un comportamento di MS Excel e non può essere modificato tramite codice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Vero se le informazioni personali possono essere rimosse dal workbook specificato.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Imposta il provider di flusso per risorse esterne, ad esempio il caricamento dei dati immagine per un'immagine di tipo "LinkToFile".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Imposta come l'applicazione visualizza le forme in questa cartella di lavoro

Vedi [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Imposta un valore che indica se la cartella di lavoro è condivisa.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Imposta un valore che indica se le schede della cartella di lavoro sono visualizzate.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Imposta il numero di cifre significative. Il valore predefinito è [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Può essere solo 15 o 17 al momento. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Questa proprietà sarà rimossa 12 mesi dopo a partire da giugno 2025. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Imposta il tipo di cifre significative per l'emissione dei valori numerici in questa cartella di lavoro. Il valore predefinito è [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Vedi [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Imposta il provider di flusso per risorse esterne.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ResourceProvider. Questa proprietà sarà rimossa 12 mesi dopo a partire da giugno 2022. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Indica se aggiornare il bordo delle celle adiacenti.

**Remarks**

Il valore predefinito è false. Per esempio: il bordo inferiore della cella A1 è aggiornato, il bordo superiore della cella A2 dovrebbe essere modificato anch'esso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Imposta come aggiornare i collegamenti esterni quando la cartella di lavoro viene aperta.

Vedi [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale.

**Remarks**

Il valore predefinito è true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


L'altezza della finestra, in unità di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


L'altezza della finestra, in unità di centimetro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


L'altezza della finestra, in unità di pollice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


La larghezza della finestra, in unità di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


La larghezza della finestra, in unità di centimetro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


La larghezza della finestra, in unità di pollice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indica se essere compatibile con WPS.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

