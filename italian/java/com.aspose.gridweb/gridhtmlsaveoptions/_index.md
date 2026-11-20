---
title: "GridHtmlSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per salvare il file html."
type: docs
url: /it/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Rappresenta le opzioni per salvare il file html.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Crea le opzioni per salvare il file html. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Crea le opzioni per salvare il file htm. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | La directory in cui verranno salvati i file allegati. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella dei file nella cache è usata per memorizzare alcuni dati di grandi dimensioni. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getDefaultFontName()](#getDefaultFontName--) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [getEncoding()](#getEncoding--) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indica se esportare l'intero workbook in un file html. |
| [getExportArea()](#getExportArea--) | Ottiene l'area CellArea da esportare del foglio di lavoro attivo corrente. |
| [getExportGridLines()](#getExportGridLines--) | Indicazione se esportare le linee della griglia. Il valore predefinito è false. |
| [getExportHeadings()](#getExportHeadings--) | Indica se esportare le intestazioni durante il salvataggio del file in html. Il valore predefinito è false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indica se esportare solo l'area di stampa nel file HTML. |
| [getExportSingleTab()](#getExportSingleTab--) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getPageTitle()](#getPageTitle--) | Il titolo della pagina HTML. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Analizza il tag html nella cella, ad esempio |

, come valore di cella, o come tag html, il valore predefinito è true |
| [getPresentationPreference()](#getPresentationPreference--) | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se aggiornare i dati della cache del grafico |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false. |
| [isFullPathLink()](#isFullPathLink--) | Indicazione se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | La directory in cui verranno salvati i file allegati. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella dei file nella cache è usata per memorizzare alcuni dati di grandi dimensioni. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indica se esportare l'intero workbook in un file html. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Imposta l'area CellArea di esportazione del foglio di lavoro attivo corrente. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indicazione se esportare le linee della griglia. Il valore predefinito è false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indica se esportare le intestazioni durante il salvataggio del file in html. Il valore predefinito è false. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indica se esportare solo l'area di stampa nel file HTML. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indicazione se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Il titolo della pagina HTML. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Analizza il tag html nella cella, ad esempio |

, come valore di cella, o come tag html, il valore predefinito è true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se aggiornare i dati della cache del grafico |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Crea le opzioni per salvare il file html.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Crea le opzioni per salvare il file htm.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Il formato di salvataggio del file. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream HTML.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Specifica il prefisso Url dei file allegati, come le immagini nel file HTML. Solo per il salvataggio in stream HTML.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella dei file nella cache è usata per memorizzare alcuni dati di grandi dimensioni.

**Returns:**
java.lang.String
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indica se esportare l'intero workbook in un file html.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Ottiene l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in html.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indicazione se esportare le linee della griglia. Il valore predefinito è false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indica se esportare le intestazioni durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare il file html in excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indica se esportare solo l'area di stampa nel file HTML. Il valore predefinito è false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indica se esportare la singola scheda quando il file contiene solo un foglio di lavoro. Il valore predefinito è false.

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
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Il titolo della pagina html. Solo per il salvataggio su stream html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Analizza il tag html nella cella, ad esempio

, come valore di cella, o come tag html, il valore predefinito è true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica se aggiornare i dati della cache del grafico

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato di salvataggio del file.

Vedi [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica se ordinare i nomi definiti prima di salvare il file.

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Specifica il prefisso Url dei file allegati, come le immagini nel file HTML. Solo per il salvataggio in stream HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La cartella dei file nella cache è usata per memorizzare alcuni dati di grandi dimensioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indica se esportare l'intero workbook in un file html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Imposta l'area CellArea da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Indicazione se esportare le linee della griglia. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Indica se esportare le intestazioni durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare il file html in excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indica se esportare solo l'area di stampa nel file HTML. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Indica se esportare la singola scheda quando il file contiene solo un foglio di lavoro. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.

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

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Il titolo della pagina html. Solo per il salvataggio su stream html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Analizza il tag html nella cella, ad esempio

, come valore di cella, o come tag html, il valore predefinito è true

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se aggiornare i dati della cache del grafico

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

