---
title: "RevisionCellComment"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre yorum değişikliğiyle ilgili bir revizyon kaydını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Hücre yorum değişikliğiyle ilgili bir revizyon kaydını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Revizyonun eylem tipini alır. |
| [getCellName()](#getCellName--) | Hücrenin adını alır. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Yorumu içeren sütunun indeksini alır. |
| [getId()](#getId--) | Bu revizyonun numarasını alır. |
| [getNewLength()](#getNewLength--) | Bu revizyon yapılmadan önce yorumun uzunluğunu alır. |
| [getOldLength()](#getOldLength--) | Bu revizyonda eklenen yorum metninin uzunluğunu alır. |
| [getRow()](#getRow--) | Yorumu içeren satırın indeksini alır. |
| [getType()](#getType--) | Revizyonun tipini alır. |
| [getWorksheet()](#getWorksheet--) | Çalışma sayfasını alır. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Eski bir yorum olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Hücrenin adını alır. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Revizyonun eylem tipini alır.

Bak [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
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


Yorumu içeren sütunun indeksini alır.

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
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Bu revizyon yapılmadan önce yorumun uzunluğunu alır.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Bu revizyonda eklenen yorum metninin uzunluğunu alır.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Yorumu içeren satırın indeksini alır.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Revizyonun tipini alır.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Eski bir yorum olup olmadığını gösterir.

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Hücrenin adını alır.

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

