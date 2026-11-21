---
title: "RevisionCellChange"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücreleri değiştiren revizyonu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Hücreleri değiştiren revizyonu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Hücrenin adını alır. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hücrenin sütun indeksini alır. |
| [getId()](#getId--) | Bu revizyonun numarasını alır. |
| [getNewFormula()](#getNewFormula--) | Eski formülü alır. |
| [getNewStyle()](#getNewStyle--) | Hücrenin yeni stilini alır. |
| [getNewValue()](#getNewValue--) | Hücrenin yeni değerini alır. |
| [getOldFormula()](#getOldFormula--) | Eski formülü alır. |
| [getOldStyle()](#getOldStyle--) | Hücrenin eski stilini alır. |
| [getOldValue()](#getOldValue--) | Hücrenin eski değerini alır. |
| [getRow()](#getRow--) | Hücrenin satır indeksini alır. |
| [getType()](#getType--) | Revizyon türünü temsil eder. |
| [getWorksheet()](#getWorksheet--) | Çalışma sayfasını alır. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Bu hücrenin yeni biçimlendirilip biçimlendirilmediğini gösterir. |
| [isOldFormatted()](#isOldFormatted--) | Bu hücrenin eski biçimlendirilip biçimlendirilmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCellName() {#getCellName--}
```
public String getCellName()
```


Hücrenin adını alır.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hücrenin sütun indeksini alır.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Bu revizyonun numarasını alır.

**Remarks**

Sıfır, bu revizyonun kimlik içermediği anlamına gelir.

**Returns:**
int
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Eski formülü alır.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Hücrenin yeni stilini alır.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Hücrenin yeni değerini alır.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Eski formülü alır.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Hücrenin eski stilini alır.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Hücrenin eski değerini alır.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Hücrenin satır indeksini alır.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Revizyon türünü temsil eder.

Bak [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Çalışma sayfasını alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Bu hücrenin yeni biçimlendirilip biçimlendirilmediğini gösterir.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Bu hücrenin eski biçimlendirilip biçimlendirilmediğini gösterir.

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

