---
title: "GridUpdateMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Güncelleme işleminin değişimini izlemek için kullanıcı monitörü."
type: docs
url: /tr/java/com.aspose.gridjs/gridupdatemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridUpdateMonitor
```

Güncelleme işleminin değişimini izlemek için kullanıcı monitörü.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridUpdateMonitor()](#GridUpdateMonitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [afterUpdate(String op, String uid, ArrayList cells)](#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-) | güncelleme işleminden sonra |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridUpdateMonitor() {#GridUpdateMonitor--}
```
public GridUpdateMonitor()
```


### afterUpdate(String op, String uid, ArrayList cells) {#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-}
```
public abstract void afterUpdate(String op, String uid, ArrayList cells)
```


güncelleme işleminden sonra

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| op | java.lang.String | Güncelleme işlemi için JSON dizesi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| cells | java.util.ArrayList | Güncellenmiş Hücreler listesi, stil değişikliği, değer değişikliği veya formül değişikliği olan hücreleri içerir |

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

