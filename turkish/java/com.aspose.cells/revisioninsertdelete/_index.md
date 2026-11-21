---
title: "RevisionInsertDelete"
second_title: "Aspose.Cells for Java API Referansı"
description: "Satır/sütun ekleme/silme eylemiyle ilgili bir revizyon kaydını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/revisioninsertdelete/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```

Satır/sütun ekleme/silme eylemiyle ilgili bir revizyon kaydını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Bu revizyonun eylem türünü alır. |
| [getCellArea()](#getCellArea--) | Ekleme/silme aralığını alır. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Bu revizyonun numarasını alır. |
| [getRevisions()](#getRevisions--) | Bu işlem tarafından revizyon listesini alır. |
| [getType()](#getType--) | Revizyon türünü temsil eder. |
| [getWorksheet()](#getWorksheet--) | Çalışma sayfasını alır. |
| [hashCode()](#hashCode--) |  |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Bu revizyonun eylem türünü alır.

Bak [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ekleme/silme aralığını alır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


Bu revizyonun numarasını alır.

**Remarks**

Sıfır, bu revizyonun kimlik içermediği anlamına gelir.

**Returns:**
int
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```


Bu işlem tarafından revizyon listesini alır.

**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
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

