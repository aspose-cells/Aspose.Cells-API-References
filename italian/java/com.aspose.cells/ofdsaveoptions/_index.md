---
title: "OfdSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per salvare un file OFDOpen Fixed-layout Document."
type: docs
url: /it/java/com.aspose.cells/ofdsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class OfdSaveOptions extends PaginatedSaveOptions
```

Rappresenta le opzioni per il salvataggio di un file OFD (Open Fixed-layout Document).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OfdSaveOptions()](#OfdSaveOptions--) | Crea le opzioni per salvare il file OFD. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Restituisce le impostazioni personalizzate durante il rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Restituisce la lingua di modifica predefinita. |
| [getDefaultFont()](#getDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Impostazione per il rendering del metafile Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getGridlineColor()](#getGridlineColor--) | Restituisce il colore della griglia. |
| [getGridlineType()](#getGridlineType--) | Restituisce il tipo di griglia. |
| [getIgnoreError()](#getIgnoreError--) | Indica se è necessario nascondere l'errore durante il rendering. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [getPageCount()](#getPageCount--) | Restituisce il numero di pagine da salvare. |
| [getPageIndex()](#getPageIndex--) | Restituisce l'indice basato su 0 della prima pagina da salvare. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [getPrintingPageType()](#getPrintingPageType--) | Indica quali pagine non verranno stampate. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Restituisce i comportamenti di rendering specifici per Excel da applicare. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSheetSet()](#getSheetSet--) | Ottiene i fogli da renderizzare. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getTextCrossType()](#getTextCrossType--) | Ottiene il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Imposta le impostazioni personalizzate durante il rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Imposta la lingua di modifica predefinita. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Impostazione per il rendering del metafile Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Imposta il colore delle linee della griglia. |
| [setGridlineType(int value)](#setGridlineType-int-) | Imposta il tipo di linea della griglia. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica se è necessario nascondere l'errore durante il rendering. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [setPageCount(int value)](#setPageCount-int-) | Imposta il numero di pagine da salvare. |
| [setPageIndex(int value)](#setPageIndex-int-) | Imposta l'indice basato su zero della prima pagina da salvare. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indica quali pagine non verranno stampate. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Imposta i comportamenti di rendering specifici di Excel da applicare. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Imposta i fogli da rendere. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OfdSaveOptions() {#OfdSaveOptions--}
```
public OfdSaveOptions()
```


Crea le opzioni per salvare il file OFD.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza del formato carta di pagesetup sarà ignorata, mentre le altre impostazioni di pagesetup avranno comunque effetto.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo.

**Remarks**

Il valore predefinito è true. Disabilitare questa proprietà può migliorare le prestazioni. Tuttavia, quando il font predefinito o specificato del testo/carattere non può essere usato per renderizzarlo, potrebbero comparire caratteri illeggibili (come blocchi) nel PDF generato. In tali situazioni l'utente dovrebbe mantenere questa proprietà impostata su true affinché venga cercato e utilizzato un font alternativo per renderizzare il testo invece;

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri prima.

**Remarks**

Il valore predefinito è true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Rendi il workbook vuoto dopo aver salvato il file.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Restituisce le impostazioni personalizzate durante il rendering.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Restituisce la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per visualizzare questi caratteri Unicode.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Impostazione per il rendering del metafile Emf.

Vedi [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

I file metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo i record EMF+, o solo i record EMF. Quando è impostato [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), i record EMF+ verranno analizzati durante il rendering della pagina, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Restituisce il colore della griglia.

**Remarks**

Ignorerà le impostazioni del colore delle linee della griglia nel file di origine.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Restituisce il tipo di griglia.

Vedi [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Il valore predefinito è il tipo Dotted.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indica se è necessario nascondere l'errore durante il rendering. L'errore può riguardare forme, immagini, rendering di grafici, ecc.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indica se generare una pagina vuota quando non c'è nulla da stampare.

**Remarks**

Il valore predefinito è true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Restituisce il numero di pagine da salvare.

**Remarks**

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine verranno renderizzate.

**Example**

Il seguente esempio mostra come rendere un intervallo di pagine (3 e 4) in un file Microsoft Excel in PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Restituisce l'indice basato su 0 della prima pagina da salvare.

**Remarks**

Il valore predefinito è 0.

**Example**

Il seguente esempio mostra come rendere un intervallo di pagine (3 e 4) in un file Microsoft Excel in PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Controlla/Indica l'avanzamento del processo di salvataggio della pagina.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Indica quali pagine non verranno stampate.

Vedi [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Se il contenuto nel foglio è scarso, alcune pagine saranno totalmente vuote nel file PDF di output. Se non desideri queste pagine vuote, puoi usare questa opzione per ometterle.

**Example**

Il codice seguente omette le pagine vuote o le pagine che contengono solo alcuni contenuti di stile come lo sfondo delle celle, i bordi.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Restituisce i comportamenti di rendering specifici per Excel da applicare.

Vedi [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Il valore predefinito è [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato di salvataggio del file.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ottiene i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nel workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

Il codice seguente rende solo il foglio attivo in PDF.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Ottiene il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella.

Vedi [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
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
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indica se sostituire solo il font del carattere quando il font della cella non è compatibile.

**Remarks**

Il valore predefinito è false. Proveremo prima il font predefinito di Workbook e PdfSaveOption/system per il font delle celle.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza del formato carta di pagesetup sarà ignorata, mentre le altre impostazioni di pagesetup avranno comunque effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo.

**Remarks**

Il valore predefinito è true. Disabilitare questa proprietà può migliorare le prestazioni. Tuttavia, quando il font predefinito o specificato del testo/carattere non può essere usato per renderizzarlo, potrebbero comparire caratteri illeggibili (come blocchi) nel PDF generato. In tali situazioni l'utente dovrebbe mantenere questa proprietà impostata su true affinché venga cercato e utilizzato un font alternativo per renderizzare il testo invece;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri prima.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendi il workbook vuoto dopo aver salvato il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Imposta le impostazioni personalizzate durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Imposta la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per visualizzare questi caratteri Unicode.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Impostazione per il rendering del metafile Emf.

Vedi [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

I file metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo i record EMF+, o solo i record EMF. Quando è impostato [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER), i record EMF+ verranno analizzati durante il rendering della pagina, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Indica se sostituire solo il font del carattere quando il font della cella non è compatibile.

**Remarks**

Il valore predefinito è false. Proveremo prima il font predefinito di Workbook e PdfSaveOption/system per il font delle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Imposta il colore delle linee della griglia.

**Remarks**

Ignorerà le impostazioni del colore delle linee della griglia nel file di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Imposta il tipo di linea della griglia.

Vedi [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Il valore predefinito è il tipo Dotted.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indica se è necessario nascondere l'errore durante il rendering. L'errore può riguardare forme, immagini, rendering di grafici, ecc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Indica se generare una pagina vuota quando non c'è nulla da stampare.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Imposta il numero di pagine da salvare.

**Remarks**

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine verranno renderizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Imposta l'indice basato su zero della prima pagina da salvare.

**Remarks**

Il valore predefinito è 0.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Controlla/Indica l'avanzamento del processo di salvataggio della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Indica quali pagine non verranno stampate.

Vedi [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Se il contenuto nel foglio è scarso, alcune pagine saranno totalmente vuote nel file PDF di output. Se non desideri queste pagine vuote, puoi usare questa opzione per ometterle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Imposta i comportamenti di rendering specifici di Excel da applicare.

Vedi [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Il valore predefinito è [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella.

Vedi [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

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

