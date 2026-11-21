---
title: "PivotFieldCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot tablonun farklı bölgelerindeki tüm PivotField nesnelerinin bir koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfieldcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFieldCollection extends CollectionBase
```

Pivot tablonun farklı bölgelerindeki tüm PivotField nesnelerinin bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(PivotField pivotField)](#add-com.aspose.cells.PivotField-) | Belirli tür PivotFields'e bir PivotField nesnesi ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addByBaseIndex(int baseFieldIndex)](#addByBaseIndex-int-) | Belirli tür PivotFields'e bir PivotField nesnesi ekler. |
| [clear()](#clear--) | PivotFieldCollection'ın tüm alanlarını temizle |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirli indeksteki PivotField nesnesini alır. |
| [get(String name)](#get-java.lang.String-) | Belirli isimdeki PivotField nesnesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getType()](#getType--) | PivotFields tipini alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [insert(int index, PivotField pivotField)](#insert-int-com.aspose.cells.PivotField-) | Belirli indekste bir pivot alanı ekle. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [move(int currPos, int destPos)](#move-int-int-) | PivotField'ı mevcut konumdan hedef konuma taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotField pivotField)](#remove-com.aspose.cells.PivotField-) | Alanı mevcut bölgeden kaldırır. |
| [removeAt(int index)](#removeAt-int-) | Alanı indeksine göre kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotField pivotField) {#add-com.aspose.cells.PivotField-}
```
public int add(PivotField pivotField)
```


Belirli tür PivotFields'e bir PivotField nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | bir PivotField nesnesi. |

**Returns:**
int - bu PivotFields içindeki PivotField nesnesinin indeksi.
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
### addByBaseIndex(int baseFieldIndex) {#addByBaseIndex-int-}
```
public int addByBaseIndex(int baseFieldIndex)
```


Belirli tür PivotFields'e bir PivotField nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | int | temel PivotFields içindeki alan indeksi. |

**Returns:**
int - bu PivotFields içindeki PivotField nesnesinin indeksi.
### clear() {#clear--}
```
public void clear()
```


PivotFieldCollection'ın tüm alanlarını temizle

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
public PivotField get(int index)
```


Belirli indeksteki PivotField nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### get(String name) {#get-java.lang.String-}
```
public PivotField get(String name)
```


Belirli isimdeki PivotField nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
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
### getType() {#getType--}
```
public int getType()
```


PivotFields tipini alır.

Bkz. [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
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
### insert(int index, PivotField pivotField) {#insert-int-com.aspose.cells.PivotField-}
```
public void insert(int index, PivotField pivotField)
```


Belirli indekste bir pivot alanı ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | Alan. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
### move(int currPos, int destPos) {#move-int-int-}
```
public void move(int currPos, int destPos)
```


PivotField'ı mevcut konumdan hedef konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| currPos | int | Sıfıra dayalı PivotField'ın mevcut konumu |
| destPos | int | Sıfıra dayalı PivotField'ın hedef konumu |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotField pivotField) {#remove-com.aspose.cells.PivotField-}
```
public void remove(PivotField pivotField)
```


Alanı mevcut bölgeden kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Alanı indeksine göre kaldırır. Yalnızca filtre, satır, sütun, veri bölgesi için.

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

