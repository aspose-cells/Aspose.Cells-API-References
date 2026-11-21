---
title: "SmartTagSetting"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma sayfasındaki tüm nesneyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/smarttagsetting/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SmartTagSetting extends CollectionBase
```

Çalışma sayfasındaki tüm [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Bir hücreye bir [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesi ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName)](#add-java.lang.String-) | Bir hücreye akıllı etiket ekle. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | İndeks ile bir [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesi alır. |
| [get(int row, int column)](#get-int-int-) | Hücrenin [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Hücrenin [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Bir hücreye bir [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücrenin satırı. |
| sütun | int | Hücrenin sütunu. |

**Returns:**
int - Çalışma sayfasındaki bir [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesinin dizinini döndürür.
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


Bir hücreye akıllı etiket ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |

**Returns:**
int -
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
public SmartTagCollection get(int index)
```


İndeks ile bir [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Listede bulunan [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesinin dizini. |

**Returns:**
[SmartTagCollection](../../com.aspose.cells/smarttagcollection) - 
### get(int row, int column) {#get-int-int-}
```
public SmartTagCollection get(int row, int column)
```


Hücrenin [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücrenin satır indeksi. |
| sütun | int | Hücrenin sütun dizini |

**Returns:**
[SmartTagCollection](../../com.aspose.cells/smarttagcollection) - Returns the [SmartTagCollection](../../com.aspose.cells/smarttagcollection) object of the cell. Returns null if there is no any smart tags on the cell.
### get(String cellName) {#get-java.lang.String-}
```
public SmartTagCollection get(String cellName)
```


Hücrenin [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |

**Returns:**
[SmartTagCollection](../../com.aspose.cells/smarttagcollection) - Returns the [SmartTagCollection](../../com.aspose.cells/smarttagcollection) object of the cell. Returns null if there is no any smart tags on the cell.
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


Belirtilen dizindeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin sıfır tabanlı dizini. |

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

