---
title: "ارتباط تشعبي"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل ارتباطًا تشعبيًا."
type: docs
url: /ar/java/com.aspose.cells/hyperlink/
---

**Inheritance:**
java.lang.Object
```
public class Hyperlink
```

يحتوي على الكائن الذي يمثل ارتباطًا تشعبيًا.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a hyperlink to a URL at "A1" cell
         int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
         //Getting a Hyperlink by index.
         Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
         //Setting display text of this hyperlink.
         hyperlink.setTextToDisplay("Aspose");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [delete()](#delete--) | يحذف هذا الارتباط التشعبي |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | يمثل عنوان الارتباط التشعبي. |
| [getArea()](#getArea--) | يحصل على نطاق الارتباط التشعبي. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | يحصل على نوع الارتباط. |
| [getScreenTip()](#getScreenTip--) | يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد. |
| [getTextToDisplay()](#getTextToDisplay--) | يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | يمثل عنوان الارتباط التشعبي. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```


يحذف هذا الارتباط التشعبي

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
### getAddress() {#getAddress--}
```
public String getAddress()
```


يمثل عنوان الارتباط التشعبي.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public CellArea getArea()
```


يحصل على نطاق الارتباط التشعبي.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```


يحصل على نوع الارتباط.

انظر [TargetModeType](../../com.aspose.cells/targetmodetype).

**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي.

**Returns:**
java.lang.String
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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


يمثل عنوان الارتباط التشعبي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي.

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

