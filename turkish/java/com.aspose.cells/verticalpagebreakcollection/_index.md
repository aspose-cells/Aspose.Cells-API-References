---
title: "VerticalPageBreakCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/verticalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VerticalPageBreakCollection extends CollectionBase
```

[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) nesnelerinden oluşan bir koleksiyonu kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int column)](#add-int-) | Koleksiyona dikey bir sayfa kesmesi ekler. |
| [add(int row, int column)](#add-int-int-) | Koleksiyona dikey bir sayfa kesmesi ekler. |
| [add(int startRow, int endRow, int column)](#add-int-int-int-) | Koleksiyona dikey bir sayfa kesmesi ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName)](#add-java.lang.String-) | Koleksiyona dikey bir sayfa kesmesi ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) öğesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Belirtilen hücre adıyla [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen adla VPageBreak öğesini kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int column) {#add-int-}
```
public int add(int column)
```


Koleksiyona dikey bir sayfa kesmesi ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Hücre sütun indeksi, sıfır tabanlı. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) nesne indeksi.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Koleksiyona dikey bir sayfa kesmesi ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücre satır indeksi, sıfır tabanlı. |
| sütun | int | Hücre sütun indeksi, sıfır tabanlı. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) nesne indeksi.
### add(int startRow, int endRow, int column) {#add-int-int-int-}
```
public int add(int startRow, int endRow, int column)
```


Koleksiyona dikey bir sayfa kesmesi ekler.

**Remarks**

Bu yöntem, bir yazdırma alanı içinde dikey sayfa sonu eklemek için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi, sıfır tabanlı. |
| endRow | int | Bitiş satır indeksi, sıfır tabanlı. |
| sütun | int | Sütun indeksi, sıfır tabanlı. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) nesne indeksi.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Koleksiyona dikey bir sayfa kesmesi ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

**Returns:**
int - [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


CollectionBase örneğinden tüm nesneleri kaldırır.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
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
public VerticalPageBreak get(int index)
```


Belirtilen indeksteki [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public VerticalPageBreak get(String cellName)
```


Belirtilen hücre adıyla [VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

**Returns:**
[VerticalPageBreak](../../com.aspose.cells/verticalpagebreak) - The element with the specified cell name.
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


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen adla VPageBreak öğesini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Eleman indeksi, sıfır tabanlı. |

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

