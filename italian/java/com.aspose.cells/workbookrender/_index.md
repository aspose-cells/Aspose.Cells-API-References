---
title: "WorkbookRender"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il rendering di una cartella di lavoro."
type: docs
url: /it/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Rappresenta un rendering di Workbook. Il costruttore di questa classe deve essere usato dopo la modifica di pagesetup, cell style.

**Remarks**
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Il costruttore di WorkbookRender |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [dispose()](#dispose--) | Rilascia le risorse create e utilizzate per il rendering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Ottiene il conteggio totale delle pagine del workbook. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Ottieni le dimensioni della pagina in pollici dell'immagine di output. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Renderizza una certa pagina su uno stream. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Renderizza una certa pagina su uno stream. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Renderizza una certa pagina su un file. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Renderizza l'intero workbook come immagine Tiff su uno stream. |
| [toImage(String filename)](#toImage-java.lang.String-) | Renderizza l'intero workbook come immagine Tiff su un file. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Renderizza il workbook su stampante |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Renderizza il workbook su stampante |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Renderizza il workbook su stampante |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


Il costruttore di WorkbookRender

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Indica quale workbook deve essere renderizzato. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene alcune proprietà dell'immagine di output |

### dispose() {#dispose--}
```
public void dispose()
```


Rilascia le risorse create e utilizzate per il rendering.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Ottiene il conteggio totale delle pagine del workbook.

**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Ottieni le dimensioni della pagina in pollici dell'immagine di output.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | int | L'indice della pagina parte da zero. |

**Returns:**
float[] - Dimensioni dell'immagine, [0] per larghezza e [1] per altezza
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Renderizza una certa pagina su uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | int | indica quale pagina deve essere convertita |
| stream | java.io.InputStream | lo stream dell'immagine di output |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Renderizza una certa pagina su uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | int | indica quale pagina deve essere convertita |
| stream | java.io.OutputStream | lo stream dell'immagine di output |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Renderizza una certa pagina su un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | int | indica quale pagina deve essere convertita |
| fileName | java.lang.String | nome file dell'immagine di output |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Renderizza l'intero workbook come immagine Tiff su uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | lo stream dell'immagine di output |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Renderizza l'intero workbook come immagine Tiff su un file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome file | java.lang.String | il nome file dell'immagine di output |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Renderizza il workbook su stampante

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Renderizza il workbook su stampante

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare ToPrinter(string PrinterName) e ImageOrPrintOptions.PageIndex, PageCount per impostare la prima pagina e il numero di pagine da stampare. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer" |
| printPageIndex | int | l'indice basato su zero della prima pagina da stampare, deve essere nell'intervallo [0, WorkbookRender.PageCount-1] |
| printPageCount | int | il numero di pagine da stampare, deve essere maggiore di zero |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Renderizza il workbook su stampante

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | imposta il nome del lavoro di stampa |

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

