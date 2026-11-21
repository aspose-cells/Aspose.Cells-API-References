---
title: "WorkbookRender"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en arbetsboksrendering."
type: docs
url: /sv/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Representerar en Workbook-rendering. Konstruktorn för denna klass måste användas efter ändring av sidinställning, cellstil.

**Remarks**
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Konstruktionen av WorkbookRender |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [dispose()](#dispose--) | Frigör resurser som skapats och används för rendering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Hämtar det totala sidantalet för arbetsboken. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Hämta sidstorlek i tum för utdata bilden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rendera en viss sida till en ström. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rendera en viss sida till en ström. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rendera en viss sida till en fil. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Rendera hela arbetsboken som Tiff-bild till en ström. |
| [toImage(String filename)](#toImage-java.lang.String-) | Rendera hela arbetsboken som Tiff-bild till en fil. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Rendera arbetsboken till skrivare |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Rendera arbetsboken till skrivare |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Rendera arbetsboken till skrivare |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


Konstruktionen av WorkbookRender

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Ange vilken arbetsbok som ska renderas. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions innehåller vissa egenskaper för utdata bilden |

### dispose() {#dispose--}
```
public void dispose()
```


Frigör resurser som skapats och används för rendering.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämtar det totala sidantalet för arbetsboken.

**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Hämta sidstorlek i tum för utdata bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | int | Sidindexet är baserat på noll. |

**Returns:**
float[] - Bildens sidstorlek, [0] för bredd och [1] för höjd
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


Rendera en viss sida till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | int | ange vilken sida som ska konverteras |
| stream | java.io.InputStream | strömmen för utdata bilden |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Rendera en viss sida till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | int | ange vilken sida som ska konverteras |
| stream | java.io.OutputStream | strömmen för utdata bilden |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Rendera en viss sida till en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | int | ange vilken sida som ska konverteras |
| fileName | java.lang.String | filnamn för utdata bilden |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Rendera hela arbetsboken som Tiff-bild till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | strömmen för utdata bilden |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Rendera hela arbetsboken som Tiff-bild till en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | java.lang.String | filnamnet för den utdata bilden |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Rendera arbetsboken till skrivare

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | namnet på skrivaren, till exempel: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Rendera arbetsboken till skrivare

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd istället ToPrinter(string PrinterName) och ImageOrPrintOptions.PageIndex, PageCount för att ange den första sidan och antalet sidor som ska skrivas ut. Denna egenskap kommer att tas bort 12 månader senare, sedan december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | namnet på skrivaren, till exempel: "Microsoft Office Document Image Writer" |
| printPageIndex | int | det 0-baserade indexet för den första sidan som ska skrivas ut, det måste ligga i intervallet [0, WorkbookRender.PageCount-1] |
| printPageCount | int | antalet sidor att skriva ut, det måste vara större än noll |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Rendera arbetsboken till skrivare

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | namnet på skrivaren, till exempel: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | ange namn för utskriftsjobbet |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

