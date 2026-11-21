---
title: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Java API Referansı"
description: "PdfBookmarkEntry, pdf yer imlerinde bir giriştir"
type: docs
url: /tr/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry, pdf yer işaretinde bir giriştir. Eğer mevcut örneğin Text özelliği null veya \"\" ise, mevcut örnek gizlenecek ve alt öğeler aynı seviyeye eklenecektir.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add();
         workbook.getWorksheets().add();
         Cell cellInPage1 = workbook.getWorksheets().get(0).getCells().get("A1");
         Cell cellInPage2 = workbook.getWorksheets().get(1).getCells().get("A1");
         Cell cellInPage3 = workbook.getWorksheets().get(2).getCells().get("A1");
         cellInPage1.putValue("page1");
         cellInPage2.putValue("page2");
         cellInPage3.putValue("page3");
 
         PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
         pbeRoot.setText("root");  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
         pbeRoot.setDestination(cellInPage1);
         pbeRoot.setSubEntry(new ArrayList());
         pbeRoot.setOpen(false);
 
         PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
         subPbe1.setText("section1");
         subPbe1.setDestination(cellInPage2);
 
         PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
         subPbe2.setText("section2");
         subPbe2.setDestination(cellInPage3);
 
         pbeRoot.getSubEntry().add(subPbe1);
         pbeRoot.getSubEntry().add(subPbe2);
 
         PdfSaveOptions saveOptions = new PdfSaveOptions();
         saveOptions.setBookmark(pbeRoot);
         workbook.save("output_bookmark.pdf", saveOptions);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | Yer işareti bağlantısının yönlendirildiği hücre. |
| [getDestinationName()](#getDestinationName--) | Hedefin adını alır. |
| [getSubEntry()](#getSubEntry--) | Bir yer işaretinin alt girişi. |
| [getText()](#getText--) | Yer işaretinin başlığı. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler. |
| [isOpen()](#isOpen--) | Bu özellik true olduğunda, bookmarkentry genişler, aksi takdirde daralır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | Yer işareti bağlantısının yönlendirildiği hücre. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Hedefin adını ayarlar. |
| [setOpen(boolean value)](#setOpen-boolean-) | Bu özellik true olduğunda, bookmarkentry genişler, aksi takdirde daralır. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | Bir yer işaretinin alt girişi. |
| [setText(String value)](#setText-java.lang.String-) | Yer işaretinin başlığı. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfBookmarkEntry() {#PdfBookmarkEntry--}
```
public PdfBookmarkEntry()
```


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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```


Yer işareti bağlantısının yönlendirildiği hücre.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


Hedefin adını alır.

**Remarks**

Eğer hedef adı ayarlanırsa, hedef bu adla adlandırılmış bir hedef olarak tanımlanır.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


Bir yer işaretinin alt girişi.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


Yer işaretinin başlığı.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapse() {#isCollapse--}
```
public boolean isCollapse()
```


Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


Bu özellik true olduğunda, bookmarkentry genişler, aksi takdirde daralır.

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




### setCollapse(boolean value) {#setCollapse-boolean-}
```
public void setCollapse(boolean value)
```


Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


Yer işareti bağlantısının yönlendirildiği hücre.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


Hedefin adını ayarlar.

**Remarks**

Eğer hedef adı ayarlanırsa, hedef bu adla adlandırılmış bir hedef olarak tanımlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


Bu özellik true olduğunda, bookmarkentry genişler, aksi takdirde daralır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


Bir yer işaretinin alt girişi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Yer işaretinin başlığı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

