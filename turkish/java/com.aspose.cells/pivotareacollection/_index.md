---
title: "PivotAreaCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot alanının bir listesini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotareacollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotAreaCollection extends CollectionBase
```

Pivot alanının bir listesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(CellArea cellArea)](#add-com.aspose.cells.CellArea-) | Özet tablo görünümüne dayalı bir alan ekler. |
| [add(PivotArea pivotArea)](#add-com.aspose.cells.PivotArea-) | Pivot alanı ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addPivotArea(PivotArea pivotArea)](#addPivotArea-com.aspose.cells.PivotArea-) | Bu koleksiyona pivot alanı ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Bir [PivotArea](../../com.aspose.cells/pivotarea) nesnesi alır; |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Bir pivot koşullu biçimlendirilmiş alan ayarını kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea) {#add-com.aspose.cells.CellArea-}
```
public void add(CellArea cellArea)
```


Özet tablo görünümüne dayalı bir alan ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Pivot tablo görünümüne dayalı alan. |

### add(PivotArea pivotArea) {#add-com.aspose.cells.PivotArea-}
```
public int add(PivotArea pivotArea)
```


Pivot alanı ekler.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen AddPivotArea() yöntemini kullanın. Bu yöntem, Aralık 2025'ten itibaren 6 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Pivot alanı. |

**Returns:**
int -
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
### addPivotArea(PivotArea pivotArea) {#addPivotArea-com.aspose.cells.PivotArea-}
```
public int addPivotArea(PivotArea pivotArea)
```


Bu koleksiyona pivot alanı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) |  |

**Returns:**
int - bu koleksiyonda eklenen pivot alanının dizini
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
public PivotArea get(int index)
```


Bir [PivotArea](../../com.aspose.cells/pivotarea) nesnesi alır;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[PivotArea](../../com.aspose.cells/pivotarea) - 
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


Bir pivot koşullu biçimlendirilmiş alan ayarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks |

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

