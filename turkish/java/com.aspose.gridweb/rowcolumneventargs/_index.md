---
title: "RowColumnEventArgs"
second_title: "Aspose.Cells for Java API Referansı"
description: "Satır/sütun olayları için veri sağlar."
type: docs
url: /tr/java/com.aspose.gridweb/rowcolumneventargs/
---

**Inheritance:**
java.lang.Object
```
public class RowColumnEventArgs
```

Satır/sütun olayları için veri sağlar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgument()](#getArgument--) | Olayın argümanı. |
| [getClass()](#getClass--) |  |
| [getNum()](#getNum--) | Satır veya sütun numarası, sıfırdan başlar. |
| [getType()](#getType--) | Satır veya sütun tipi. |
| [hashCode()](#hashCode--) |  |
| [isCancel()](#isCancel--) | İşlemi iptal edelim mi. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rejectOperation()](#rejectOperation--) | Silme işlemlerini iptal etmek için RowDeleting/ColumnDeleting olay işleyicilerinde bu yöntemi çağırın. |
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
### getArgument() {#getArgument--}
```
public Object getArgument()
```


Olayın argümanı.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getNum() {#getNum--}
```
public int getNum()
```


Satır veya sütun numarası, sıfırdan başlar.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Satır veya sütun tipi.

Bakın [RowColumnType](../../com.aspose.gridweb/rowcolumntype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCancel() {#isCancel--}
```
public boolean isCancel()
```


İşlemi iptal edelim mi.

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




### rejectOperation() {#rejectOperation--}
```
public void rejectOperation()
```


Silme işlemlerini iptal etmek için RowDeleting/ColumnDeleting olay işleyicilerinde bu yöntemi çağırın.

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

