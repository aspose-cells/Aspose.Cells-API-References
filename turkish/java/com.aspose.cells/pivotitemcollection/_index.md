---
title: "PivotItemCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotField içindeki tüm nesneleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotitemcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotItemCollection extends CollectionBase
```

PivotField içindeki tüm [PivotItem](../../com.aspose.cells/pivotitem) nesnelerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [changeitemsOrder(int sourceIndex, int destIndex)](#changeitemsOrder-int-int-) | İki öğenin sırasını doğrudan değiştirir. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirli indeksteki PivotItem nesnesini alır. |
| [get(String itemValue)](#get-java.lang.String-) | Belirli adla [PivotItem](../../com.aspose.cells/pivotitem) alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetail(boolean isHiddenDetail)](#hideAllDetail-boolean-) | Bir pivot alanındaki tüm PivotItem'ların tüm detaylarını gizleyip gizlemeyeceğini ayarlar. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [swapItem(int index1, int index2)](#swapItem-int-int-) | İki öğeyi doğrudan değiştir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### changeitemsOrder(int sourceIndex, int destIndex) {#changeitemsOrder-int-int-}
```
public void changeitemsOrder(int sourceIndex, int destIndex)
```


İki öğenin sırasını doğrudan değiştirir.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotItemCollection.SwapItem() yöntemini kullanın. Bu yöntem, Temmuz 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | int | Geçerli dizin |
| destIndex | int | Hedef dizin |

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
public PivotItem get(int index)
```


Belirli indeksteki PivotItem nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
### get(String itemValue) {#get-java.lang.String-}
```
public PivotItem get(String itemValue)
```


Belirli adla [PivotItem](../../com.aspose.cells/pivotitem) alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| itemValue | java.lang.String |  |

**Returns:**
[PivotItem](../../com.aspose.cells/pivotitem)
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
### hideAllDetail(boolean isHiddenDetail) {#hideAllDetail-boolean-}
```
public void hideAllDetail(boolean isHiddenDetail)
```


Bir pivot alanındaki tüm PivotItem'ların tüm detaylarını gizleyip gizlemeyeceğini ayarlar. Bu, alanı daraltıp genişletmek anlamına gelir.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.HideAllDetails() ve ShowAllDetails() yöntemlerini kullanın. Bu yöntem, Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isHiddenDetail | boolean | Pivot alanının detayını gizleyip gizlemeyeceği. |

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

### swapItem(int index1, int index2) {#swapItem-int-int-}
```
public void swapItem(int index1, int index2)
```


İki öğeyi doğrudan değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index1 | int |  |
| index2 | int |  |

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

