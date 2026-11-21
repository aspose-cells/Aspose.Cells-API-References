---
title: "SheetRender"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en arbetsbladsrendering som kan rendera arbetsblad till olika bilder såsom BMP PNG JPEG TIFF.."
type: docs
url: /sv/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Representerar en arbetsbladsrendering som kan rendera arbetsblad till olika bilder såsom (BMP, PNG, JPEG, TIFF..) Konstruktorn för denna klass måste användas efter ändring av sidinställning, cellstil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | konstruktionen av SheetRender kräver arbetsblad och ImageOrPrintOptions som parametrar |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [dispose()](#dispose--) | Frigör resurser som skapats och används för rendering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Hämtar det totala sidantalet för det aktuella arbetsbladet. |
| [getPageScale()](#getPageScale--) | Hämtar beräknad sidskala för bladet. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Hämta sidstorlek i tum för utdata bilden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Rendera en viss sida till en ström. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Rendera en viss sida till en ström. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Rendera en viss sida till en fil. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Rendera kalkylblad till skrivare |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Rendera kalkylblad till skrivare |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Rendera kalkylblad till skrivare |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Rendera hela kalkylbladet som Tiff Image till ström. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


konstruktionen av SheetRender kräver arbetsblad och ImageOrPrintOptions som parametrar

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Ange vilket kalkylblad som ska renderas. |
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


Hämtar det totala sidantalet för det aktuella arbetsbladet.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Hämtar beräknad sidskala för bladet. Returnerar den inställda skalan om [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) är satt. Annars returneras den beräknade skalan enligt [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) och [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

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

**Example**

Följande kod skriver ut den första sidan av det första bladet till png-bild.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | int | ange vilken sida som ska konverteras |
| fileName | java.lang.String | filnamn för utdata bilden |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Rendera kalkylblad till skrivare

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | namnet på skrivaren, till exempel: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Rendera kalkylblad till skrivare

**Remarks**

OBS: Den här metoden är nu föråldrad. Använd istället ToPrinter(string PrinterName) och ImageOrPrintOptions.PageIndex, PageCount för att ange den första sidan och antalet sidor som ska skrivas ut. Denna egenskap kommer att tas bort 12 månader senare, sedan december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | namnet på skrivaren, till exempel: "Microsoft Office Document Image Writer" |
| printPageIndex | int | det 0-baserade indexet för den första sidan att skriva ut, det måste ligga i intervallet [0, SheetRender.PageCount-1] |
| printPageCount | int | antalet sidor att skriva ut, det måste vara större än noll |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Rendera kalkylblad till skrivare

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
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Rendera hela kalkylbladet som Tiff Image till ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | strömmen för utdata bilden |

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

