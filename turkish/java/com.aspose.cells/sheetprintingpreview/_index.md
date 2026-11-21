---
title: "SheetPrintingPreview"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma sayfası yazdırma önizlemesi."
type: docs
url: /tr/java/com.aspose.cells/sheetprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class SheetPrintingPreview
```

Çalışma sayfası yazdırma önizlemesi.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)](#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | SheetPrintingPreview'in yapısı |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Bu çalışma sayfasının toplam sayfa sayısını değerlendirin. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options) {#SheetPrintingPreview-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```


SheetPrintingPreview'in yapısı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Yazdırılacak elektronik tabloyu belirtin. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions, çıktının bazı özelliklerini içerir. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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
### getEvaluatedPageCount() {#getEvaluatedPageCount--}
```
public int getEvaluatedPageCount()
```


Bu çalışma sayfasının toplam sayfa sayısını değerlendirin.

**Example**

Aşağıdaki kod, bir çalışma sayfasının sayfa sayısını almanın en hızlı yolunu gösterir.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in worksheet.
         System.out.println(sheetPrintingPreview.getEvaluatedPageCount());
```

**Returns:**
int
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

