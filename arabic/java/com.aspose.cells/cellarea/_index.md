---
title: "CellArea"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مساحة من الخلايا."
type: docs
url: /ar/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

يمثل مساحة من الخلايا.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## حقول

| حقل | الوصف |
| --- | --- |
| [EndColumn](#EndColumn) | يحصل أو يضبط العمود النهائي لهذه المنطقة. |
| [EndRow](#EndRow) | يحصل أو يضبط الصف النهائي لهذه المنطقة. |
| [StartColumn](#StartColumn) | يحصل أو يضبط العمود الابتدائي لهذه المنطقة. |
| [StartRow](#StartRow) | يحصل أو يضبط الصف الابتدائي لهذه المنطقة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | قارن كائنين من نوع CellArea وفقًا للزاوية العلوية اليسرى لهما. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | ينشئ مساحة خلية. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | ينشئ مساحة خلية. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن مساحة الخلية الحالي. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


يحصل أو يضبط العمود النهائي لهذه المنطقة.

### EndRow {#EndRow}
```
public int EndRow
```


يحصل أو يضبط الصف النهائي لهذه المنطقة.

### StartColumn {#StartColumn}
```
public int StartColumn
```


يحصل أو يضبط العمود الابتدائي لهذه المنطقة.

### StartRow {#StartRow}
```
public int StartRow
```


يحصل أو يضبط الصف الابتدائي لهذه المنطقة.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


قارن كائنين من نوع CellArea وفقًا للزاوية العلوية اليسرى لهما.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - إذا كانت الزاويتان في صفوف مختلفة، فقارن فهرس الصف الخاص بهما. وإلا قارن فهرس العمود. إذا كانت الزاويتان متطابقتين، سيتم إرجاع 0.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


ينشئ مساحة خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية. |
| endRow | int | صف النهاية. |
| endColumn | int | عمود النهاية. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


ينشئ مساحة خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startCellName | java.lang.String | الخلية العلوية اليسرى للنطاق. |
| endCellName | java.lang.String | الخلية السفلية اليمنى للنطاق. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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


يرجع سلسلة تمثل كائن مساحة الخلية الحالي.

**Returns:**
java.lang.String -
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

