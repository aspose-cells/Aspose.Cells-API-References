---
title: "SheetRender"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un rendering di un foglio di lavoro che può renderizzare il foglio in varie immagini come BMP, PNG, JPEG, TIFF.."
type: docs
url: /it/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Rappresenta un rendering di un foglio di lavoro che può renderizzare il foglio in varie immagini come (BMP, PNG, JPEG, TIFF..). Il costruttore di questa classe deve essere utilizzato dopo la modifica di pageSetup e dello stile delle celle.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | la costruzione di SheetRender richiede un foglio di lavoro e ImageOrPrintOptions come parametri |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [dispose()](#dispose--) | Rilascia le risorse create e utilizzate per il rendering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Restituisce il conteggio totale delle pagine del foglio di lavoro corrente. |
| [getPageScale()](#getPageScale--) | Restituisce la scala della pagina calcolata del foglio. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Ottieni le dimensioni della pagina in pollici dell'immagine di output. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Renderizza una certa pagina su uno stream. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Renderizza una certa pagina su uno stream. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Renderizza una certa pagina su un file. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Renderizza il foglio di lavoro sulla stampante |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Renderizza il foglio di lavoro sulla stampante |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Renderizza il foglio di lavoro sulla stampante |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Renderizza l'intero foglio di lavoro come immagine Tiff nello stream. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


la costruzione di SheetRender richiede un foglio di lavoro e ImageOrPrintOptions come parametri

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Indica quale foglio di calcolo deve essere renderizzato. |
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


Restituisce il conteggio totale delle pagine del foglio di lavoro corrente.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Restituisce la scala della pagina calcolata del foglio. Restituisce la scala impostata se [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) è impostata. Altrimenti, restituisce la scala calcolata in base a [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) e [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
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

**Example**

Il codice seguente genera la prima pagina del primo foglio in un'immagine png.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | int | indica quale pagina deve essere convertita |
| fileName | java.lang.String | nome file dell'immagine di output |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Renderizza il foglio di lavoro sulla stampante

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Renderizza il foglio di lavoro sulla stampante

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare ToPrinter(string PrinterName) e ImageOrPrintOptions.PageIndex, PageCount per impostare la prima pagina e il numero di pagine da stampare. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2021. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | il nome della stampante, ad esempio: "Microsoft Office Document Image Writer" |
| printPageIndex | int | l'indice basato su zero della prima pagina da stampare, deve essere nell'intervallo [0, SheetRender.PageCount-1] |
| printPageCount | int | il numero di pagine da stampare, deve essere maggiore di zero |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Renderizza il foglio di lavoro sulla stampante

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
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Renderizza l'intero foglio di lavoro come immagine Tiff nello stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | lo stream dell'immagine di output |

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

