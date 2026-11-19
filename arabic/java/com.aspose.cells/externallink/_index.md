---
title: "ExternalLink"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل رابطًا خارجيًا في مصنف."
type: docs
url: /ar/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

يمثل رابطًا خارجيًا في مصنف.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | يضيف اسمًا خارجيًا. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | يمثل مصدر البيانات للرابط الخارجي. |
| [getOriginalDataSource()](#getOriginalDataSource--) | يمثل مصدر البيانات المخزن للرابط الخارجي. |
| [getPathType()](#getPathType--) | احصل على نوع المسار لهذا الرابط الخارجي |
| [getType()](#getType--) | يحصل على نوع الرابط الخارجي. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | يشير إلى ما إذا كان هذا الرابط الخارجي مُشارًا إليه من قبل الآخرين. |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هذا الرابط الخارجي مرئيًا في MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | يمثل مصدر البيانات للرابط الخارجي. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | يمثل مصدر البيانات المخزن للرابط الخارجي. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


يضيف اسمًا خارجيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص الاسم الخارجي. إذا كان الاسم الخارجي ينتمي إلى ورقة عمل، يجب أن يكون النص على الشكل Sheet1!Text. |
| referTo | java.lang.String | الخاصية referTo للاسم الخارجي. يجب أن تكون خلية أو نطاق. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


يمثل مصدر البيانات للرابط الخارجي.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


يمثل مصدر البيانات المخزن للرابط الخارجي.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


احصل على نوع المسار لهذا الرابط الخارجي

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع الرابط الخارجي.

انظر [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


يشير إلى ما إذا كان هذا الرابط الخارجي مُشارًا إليه من قبل الآخرين.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يشير إلى ما إذا كان هذا الرابط الخارجي مرئيًا في MS Excel.

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




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


يمثل مصدر البيانات للرابط الخارجي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


يمثل مصدر البيانات المخزن للرابط الخارجي.

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

