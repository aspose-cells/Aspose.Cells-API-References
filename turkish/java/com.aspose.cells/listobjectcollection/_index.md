---
title: "ListObjectCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma sayfasındaki nesnelerin bir koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/listobjectcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ListObjectCollection extends CollectionBase
```

Çalışma sayfasındaki [ListObject](../../com.aspose.cells/listobject) nesnelerinin bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#add-int-int-int-int-boolean-) | Çalışma sayfasına bir ListObject ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String startCell, String endCell, boolean hasHeaders)](#add-java.lang.String-java.lang.String-boolean-) | Çalışma sayfasına bir ListObject ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | ListObject'i indeksine göre alır. |
| [get(String tableName)](#get-java.lang.String-) | Belirtilen adla ListObject'i alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | İndeks ile [ListObject](../../com.aspose.cells/listobject) kaldır. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Tabloların tüm sütun adlarını günceller. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#add-int-int-int-int-boolean-}
```
public int add(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Çalışma sayfasına bir ListObject ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Liste aralığının başlangıç satırı. |
| startColumn | int | Liste aralığının başlangıç satırı. |
| endRow | int | Liste aralığının başlangıç satırı. |
| endColumn | int | Liste aralığının başlangıç satırı. |
| hasHeaders | boolean | Aralığın başlıkları olup olmadığını belirtir. |

**Returns:**
int - Yeni ListObject'in indeksi
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
### add(String startCell, String endCell, boolean hasHeaders) {#add-java.lang.String-java.lang.String-boolean-}
```
public int add(String startCell, String endCell, boolean hasHeaders)
```


Çalışma sayfasına bir ListObject ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCell | java.lang.String | Liste aralığının başlangıç hücresi. |
| endCell | java.lang.String | Liste aralığının son hücresi. |
| hasHeaders | boolean | Aralığın başlıkları olup olmadığını belirtir. |

**Returns:**
int - Yeni ListObject'in indeksi
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
public ListObject get(int index)
```


ListObject'i indeksine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
### get(String tableName) {#get-java.lang.String-}
```
public ListObject get(String tableName)
```


Belirtilen adla ListObject'i alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableName | java.lang.String | ListObject adı. |

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - The ListObject
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


İndeks ile [ListObject](../../com.aspose.cells/listobject) kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Tabloların tüm sütun adlarını günceller.

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

