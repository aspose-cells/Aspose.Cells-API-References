---
title: "WorkbookPrintingPreview"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma kitabı yazdırma önizlemesi."
type: docs
url: /tr/java/com.aspose.cells/workbookprintingpreview/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookPrintingPreview
```

Çalışma kitabı yazdırma önizlemesi.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)](#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | WorkbookPrintingPreview'in yapısı |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEvaluatedPageCount()](#getEvaluatedPageCount--) | Bu çalışma kitabının toplam sayfa sayısını değerlendirin |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options) {#WorkbookPrintingPreview-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```


WorkbookPrintingPreview'in yapısı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Yazdırılacak çalışma kitabını belirtin. |
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


Bu çalışma kitabının toplam sayfa sayısını değerlendirin

**Example**

Aşağıdaki kod, bir çalışma kitabının sayfa sayısını almanın en hızlı yolunu gösterir.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, new ImageOrPrintOptions());
 
         //fastest way to get page count especailly when there are massive data in workbook.
         System.out.println(workbookPrintingPreview.getEvaluatedPageCount());
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

