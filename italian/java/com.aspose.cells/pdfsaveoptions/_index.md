---
title: "PdfSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per il salvataggio del file pdf."
type: docs
url: /it/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

Rappresenta le opzioni per il salvataggio del file pdf.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Crea le opzioni per salvare il file PDF. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [getBookmark()](#getBookmark--) | Restituisce l'oggetto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCalculateFormula()](#getCalculateFormula--) | Indica se calcolare le formule prima di salvare il file pdf. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCompliance()](#getCompliance--) | Ottiene il livello di conformità agli standard PDF per i documenti di output. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getCreatedTime()](#getCreatedTime--) | Ottiene l'ora di generazione del documento pdf. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Ottiene un valore che determina il modo in cui [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) vengono esportati nel file PDF. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Restituisce le impostazioni personalizzate durante il rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Restituisce la lingua di modifica predefinita. |
| [getDefaultFont()](#getDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Indica se incorporare gli allegati per gli oggetti Ole in Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True per incorporare i font TrueType. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Impostazione per il rendering del metafile Emf. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Indica se esportare la struttura del documento. |
| [getFontEncoding()](#getFontEncoding--) | Ottiene la codifica del font incorporato nel pdf. |
| [getGridlineColor()](#getGridlineColor--) | Restituisce il colore della griglia. |
| [getGridlineType()](#getGridlineType--) | Restituisce il tipo di griglia. |
| [getIgnoreError()](#getIgnoreError--) | Indica se è necessario nascondere l'errore durante il rendering. |
| [getImageType()](#getImageType--) | Rappresenta il tipo di immagine durante la conversione del grafico e della forma. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [getOptimizationType()](#getOptimizationType--) | Ottiene il tipo di ottimizzazione PDF. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [getPageCount()](#getPageCount--) | Restituisce il numero di pagine da salvare. |
| [getPageIndex()](#getPageIndex--) | Restituisce l'indice basato su 0 della prima pagina da salvare. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [getPdfCompression()](#getPdfCompression--) | Indica l'algoritmo di compressione |
| [getPrintingPageType()](#getPrintingPageType--) | Indica quali pagine non verranno stampate. |
| [getProducer()](#getProducer--) | Ottiene il produttore del documento PDF generato. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Restituisce i comportamenti di rendering specifici per Excel da applicare. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSecurityOptions()](#getSecurityOptions--) | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf. |
| [getSheetSet()](#getSheetSet--) | Ottiene i fogli da renderizzare. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getTextCrossType()](#getTextCrossType--) | Ottiene il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [getWatermark()](#getWatermark--) | Ottiene la filigrana per l'output. |
| [getZoomBehavior()](#getZoomBehavior--) | Ottiene la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. |
| [getZoomFactor()](#getZoomFactor--) | Ottiene la percentuale di zoom utilizzata quando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) è [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Imposta l'oggetto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica se calcolare le formule prima di salvare il file pdf. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indica se verificare la compatibilità dei caratteri per ogni carattere nel testo. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCompliance(int value)](#setCompliance-int-) | Imposta il livello di conformità agli standard PDF per i documenti di output. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Imposta l'ora di generazione del documento pdf. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Imposta un valore che determina il modo in cui [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) vengono esportati nel file PDF. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Imposta le impostazioni personalizzate durante il rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Imposta la lingua di modifica predefinita. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Indica se incorporare gli allegati per gli oggetti Ole in Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | True per incorporare i font TrueType. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Impostazione per il rendering del metafile Emf. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Indica se esportare la struttura del documento. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Imposta la codifica del font incorporato nel pdf. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Imposta il colore delle linee della griglia. |
| [setGridlineType(int value)](#setGridlineType-int-) | Imposta il tipo di linea della griglia. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indica se è necessario nascondere l'errore durante il rendering. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Imposta i PPI (pixel per pollice) desiderati per le immagini ricampionabili e la qualità JPEG. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Rappresenta il tipo di immagine durante la conversione del grafico e della forma. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Imposta il tipo di ottimizzazione PDF. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [setPageCount(int value)](#setPageCount-int-) | Imposta il numero di pagine da salvare. |
| [setPageIndex(int value)](#setPageIndex-int-) | Imposta l'indice basato su zero della prima pagina da salvare. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Indica l'algoritmo di compressione |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indica quali pagine non verranno stampate. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Imposta il produttore del documento PDF generato. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Imposta i comportamenti di rendering specifici di Excel da applicare. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Imposta i fogli da rendere. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Imposta la filigrana nell'output. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Imposta la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Imposta la percentuale di zoom utilizzata quando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) è [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Crea le opzioni per salvare il file PDF.

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
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


Restituisce l'oggetto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica se calcolare le formule prima di salvare il file pdf.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Ottiene il livello di conformità agli standard PDF per i documenti di output.

Vedi [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Il valore predefinito è Pdf17.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Ottiene l'ora di generazione del documento pdf.

**Remarks**

Se non viene impostato, sarà l'ora di generazione del PDF.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


Ottiene un valore che determina il modo in cui [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) viene esportata nel file PDF. Il valore predefinito è None.

Vedi [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
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
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Indica se la barra del titolo della finestra deve visualizzare il titolo del documento.

**Remarks**

Se false, la barra del titolo dovrebbe invece visualizzare il nome del file PDF. Il valore predefinito è false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Indica se incorporare gli allegati per gli oggetti Ole in Excel.

**Remarks**

Il valore predefinito è false. Il valore deve essere false quando è impostata la conformità PDF/A o la crittografia PDF è abilitata.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True per incorporare i font TrueType. Influisce solo sui caratteri ASCII 32-127. I font per i codici di carattere superiori a 127 sono sempre incorporati. I font sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b. Il valore predefinito è true.

**Returns:**
boolean
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
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Indica se esportare la struttura del documento.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


Ottiene la codifica del font incorporato nel pdf.

Vedi [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Il valore predefinito è [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Returns:**
int
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
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Rappresenta il tipo di immagine durante la conversione del grafico e della forma.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
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
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


Ottiene il tipo di ottimizzazione PDF.

Vedi [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Il valore predefinito è [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Returns:**
int
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
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Indica l'algoritmo di compressione

Vedi [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
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
### getProducer() {#getProducer--}
```
public String getProducer()
```


Ottiene il produttore del documento PDF generato.

**Remarks**

Se il valore è null o una LICENSE valida non è impostata, verrà utilizzata la stringa Aspose.Cells vVERSION.

**Returns:**
java.lang.String
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
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf.

**Example**

Il codice seguente imposta il permesso di stampa della risoluzione in altezza per il PDF di output.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
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
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Ottiene la filigrana per l'output.

**Example**

Il codice seguente imposta la filigrana nel PDF di output.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Ottiene la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. Il valore predefinito è [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Vedi [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Ottiene la percentuale di zoom utilizzata quando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) è [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Questa proprietà è ignorata a meno che [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) sia [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Returns:**
int
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

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


Imposta l'oggetto [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

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

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica se calcolare le formule prima di salvare il file pdf.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Imposta il livello di conformità agli standard PDF per i documenti di output.

Vedi [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Il valore predefinito è Pdf17.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Imposta l'ora di generazione del documento pdf.

**Remarks**

Se non viene impostato, sarà l'ora di generazione del PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


Imposta un valore che determina il modo in cui [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) viene esportata nel file PDF. Il valore predefinito è None.

Vedi [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Indica se la barra del titolo della finestra deve visualizzare il titolo del documento.

**Remarks**

Se false, la barra del titolo dovrebbe invece visualizzare il nome del file PDF. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Indica se incorporare gli allegati per gli oggetti Ole in Excel.

**Remarks**

Il valore predefinito è false. Il valore deve essere false quando è impostata la conformità PDF/A o la crittografia PDF è abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True per incorporare i font TrueType. Influisce solo sui caratteri ASCII 32-127. I font per i codici di carattere superiori a 127 sono sempre incorporati. I font sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Indica se esportare la struttura del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


Imposta la codifica del font incorporato nel pdf.

Vedi [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Il valore predefinito è [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Imposta il PPI (pixel per pollice) desiderato per il ridimensionamento delle immagini e la qualità JPEG. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata, e le immagini con un PPI superiore a quello specificato saranno ridimensionate.

**Example**

Il codice seguente imposta il PPI desiderato a 96 e la qualità JPEG a 80 per le immagini nel PDF di output.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredPPI | int | Pixel desiderati per pollice. 220 alta qualità. 150 qualità per schermo. 96 qualità per email. |
| jpegQuality | int | Qualità JPEG da 0 a 100%. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Rappresenta il tipo di immagine durante la conversione del grafico e della forma.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


Imposta il tipo di ottimizzazione PDF.

Vedi [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Il valore predefinito è [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Indica l'algoritmo di compressione

Vedi [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Imposta il produttore del documento PDF generato.

**Remarks**

Se il valore è null o una LICENSE valida non è impostata, verrà utilizzata la stringa Aspose.Cells vVERSION.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Imposta la filigrana nell'output.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Imposta la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. Il valore predefinito è [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Vedi [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Imposta la percentuale di zoom utilizzata quando [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) è [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Questa proprietà è ignorata a meno che [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) sia [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

