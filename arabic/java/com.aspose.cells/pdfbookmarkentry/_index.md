---
title: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Java API Reference"
description: "PdfBookmarkEntry هو إدخال في إشارة مرجعية PDF."
type: docs
url: /ar/java/com.aspose.cells/pdfbookmarkentry/
---

**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```

PdfBookmarkEntry هو عنصر في إشارة مرجعية PDF. إذا كانت خاصية Text للنسخة الحالية null أو \"\", سيتم إخفاء النسخة الحالية وسيتم إدراج الأطفال في المستوى الحالي.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | الخلية التي يرتبط بها رابط الإشارة المرجعية. |
| [getDestinationName()](#getDestinationName--) | يحصل على اسم الوجهة. |
| [getSubEntry()](#getSubEntry--) | عنصر فرعي لإشارة مرجعية. |
| [getText()](#getText--) | عنوان إشارة مرجعية. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | عند تكون هذه الخاصية true، سيُطوى عنصر الإشارة المرجعية، وإلا سيتوسع. |
| [isOpen()](#isOpen--) | عند تكون هذه الخاصية true، سيتوسع عنصر الإشارة المرجعية، وإلا سيُطوى. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | عند تكون هذه الخاصية true، سيُطوى عنصر الإشارة المرجعية، وإلا سيتوسع. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | الخلية التي يرتبط بها رابط الإشارة المرجعية. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | يضبط اسم الوجهة. |
| [setOpen(boolean value)](#setOpen-boolean-) | عند تكون هذه الخاصية true، سيتوسع عنصر الإشارة المرجعية، وإلا سيُطوى. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | عنصر فرعي لإشارة مرجعية. |
| [setText(String value)](#setText-java.lang.String-) | عنوان إشارة مرجعية. |
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
| معامل | نوع | الوصف |
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


الخلية التي يرتبط بها رابط الإشارة المرجعية.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```


يحصل على اسم الوجهة.

**Remarks**

إذا تم ضبط اسم الوجهة، فستُعرّف الوجهة كوجهة مسماة بهذا الاسم.

**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```


عنصر فرعي لإشارة مرجعية.

**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```


عنوان إشارة مرجعية.

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


عند تكون هذه الخاصية true، سيُطوى عنصر الإشارة المرجعية، وإلا سيتوسع.

**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```


عند تكون هذه الخاصية true، سيتوسع عنصر الإشارة المرجعية، وإلا سيُطوى.

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


عند تكون هذه الخاصية true، سيُطوى عنصر الإشارة المرجعية، وإلا سيتوسع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```


الخلية التي يرتبط بها رابط الإشارة المرجعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |

### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```


يضبط اسم الوجهة.

**Remarks**

إذا تم ضبط اسم الوجهة، فستُعرّف الوجهة كوجهة مسماة بهذا الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```


عند تكون هذه الخاصية true، سيتوسع عنصر الإشارة المرجعية، وإلا سيُطوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```


عنصر فرعي لإشارة مرجعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.ArrayList |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


عنوان إشارة مرجعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

