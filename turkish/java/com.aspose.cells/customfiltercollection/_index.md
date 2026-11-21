---
title: "CustomFilterCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Özel filtreleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/customfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomFilterCollection extends CollectionBase
```

Özel filtreleri temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomFilterCollection()](#CustomFilterCollection--) | Yeni bir örnek oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-java.lang.Object-boolean-int-java.lang.Object-) | Bir listeyi özel ölçütlerle filtreler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirli indeksteki özel filtreyi alır. |
| [getAnd()](#getAnd--) | İki ölçütün "and" ilişkisine sahip olup olmadığını gösterir. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [setAnd(boolean value)](#setAnd-boolean-) | İki ölçütün "and" ilişkisine sahip olup olmadığını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFilterCollection() {#CustomFilterCollection--}
```
public CustomFilterCollection()
```


Yeni bir örnek oluşturur.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, FilterColumn.FilterType'ı FilterType.CustomFilters olarak ayarlayın ve ardından FilterColumn.CustomFilters'ı alın. Bu özellik, Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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
### custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Bir listeyi özel ölçütlerle filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filtre operatör türü |
| criteria1 | java.lang.Object | Özel kriter |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filtre operatör türü |
| criteria2 | java.lang.Object | Özel kriter |

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
public CustomFilter get(int index)
```


Belirli indeksteki özel filtreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[CustomFilter](../../com.aspose.cells/customfilter) - 
### getAnd() {#getAnd--}
```
public boolean getAnd()
```


İki ölçütün "and" ilişkisine sahip olup olmadığını gösterir.

**Returns:**
boolean
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

### setAnd(boolean value) {#setAnd-boolean-}
```
public void setAnd(boolean value)
```


İki ölçütün "and" ilişkisine sahip olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

