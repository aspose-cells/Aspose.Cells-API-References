---
title: "GridNameCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Bir dizi [GridName](../../com.aspose.gridweb/gridname) nesnesini kapsüller.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Belirtilen sayfada yeni bir ad tanımlar. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Yeni bir küresel ad tanımlar. |
| [clear()](#clear--) | Tüm Adları kaldırır; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [GridName](../../com.aspose.gridweb/gridname) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Yineleyicinin boyutunu alır |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Satırların yineleyicisini alır |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Adların bir dizisini kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirli indeksteki adı kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Belirtilen sayfada yeni bir ad tanımlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Adın uygulandığı sayfa indeksi. |
| metin | java.lang.String | Ad metni. Sayfa adı içeremez. |
| refersTo | java.lang.String | Adın başvuracağı şekilde tanımlanan formül. Sayfa adı içermelidir. örn.'sheet hello!'A1:B2. |

**Returns:**
int - Ad nesnesi indeksi.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Yeni bir küresel ad tanımlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Ad metni. Sayfa adı içerebilir. |
| refersTo | java.lang.String | Adın başvuracağı şekilde tanımlanan formül. Bir sayfa adı içermelidir. örn.'sheet hello!'A1:B2. |

**Returns:**
int - Ad nesnesi indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm Adları kaldırır;

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
### get(int index) {#get-int-}
```
public GridName get(int index)
```


Belirtilen indeksteki [GridName](../../com.aspose.gridweb/gridname) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Yineleyicinin boyutunu alır

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Satırların yineleyicisini alır

**Returns:**
java.util.Iterator - Satırların yineleyicisi
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Adların bir dizisini kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adlar | java.lang.String[] | İsimlerin metni. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirli indeksteki adı kaldır.

**Remarks**

Yöntemi çağırmadan önce adın diğer formüller tarafından referans edilmediğinden emin olun. Ve eğer ad referans ediliyorsa, yalnızca Name.RefersTo özelliğini null olarak ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

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

