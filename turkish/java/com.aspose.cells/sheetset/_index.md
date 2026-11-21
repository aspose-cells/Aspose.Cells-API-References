---
title: "SheetSet"
second_title: "Aspose.Cells for Java API Referansı"
description: "bir dizi sayfayı tanımlar."
type: docs
url: /tr/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

bir dizi sayfayı tanımlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Tam sayfa indekslerine dayalı bir sayfa kümesi oluşturur. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Tam sayfa adlarına dayalı bir sayfa kümesi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Çalışma kitabının aktif sayfasını içeren bir küme alır. |
| [getAll()](#getAll--) | Çalışma kitabının tüm sayfalarını orijinal sıralarında içeren bir küme alır. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Çalışma kitabının görünür sayfalarını orijinal sıralarında içeren bir küme alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Tam sayfa indekslerine dayalı bir sayfa kümesi oluşturur.

**Remarks**

Çalışma kitabında bulunmayan bir sayfa ile karşılaşılırsa, işleme sırasında bir istisna fırlatılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndexes | int[] | sıfır tabanlı sayfa indeksleri. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Tam sayfa adlarına dayalı bir sayfa kümesi oluşturur.

**Remarks**

Çalışma kitabında bulunmayan bir sayfa ile karşılaşılırsa, işleme sırasında bir istisna fırlatılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetNames | java.lang.String[] | sayfa adları. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Çalışma kitabının aktif sayfasını içeren bir küme alır.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Çalışma kitabının tüm sayfalarını orijinal sıralarında içeren bir küme alır.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Çalışma kitabının görünür sayfalarını orijinal sıralarında içeren bir küme alır.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

