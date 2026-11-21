---
title: "TableStyleElementCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tablo stilinin tüm öğelerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/tablestyleelementcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleElementCollection extends CollectionBase
```

Tablo stilinin tüm öğelerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int type)](#add-int-) | Bir öğe ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Tablo stilinin bir öğesini indeksine göre alır. |
| [getByTableStyleElementType(int type)](#getByTableStyleElementType-int-) | Tablo stilinin öğesini öğe tipine göre alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getTableStyleElementWithIndex(int index)](#getTableStyleElementWithIndex-int-) | Tablo stilinin bir öğesini indeksine göre alır. |
| [getTableStyleElementWithType(int type)](#getTableStyleElementWithType-int-) | Tablo stilinin öğesini öğe tipine göre alır. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


Bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Öğenin tipi |

**Returns:**
int - Listedeki öğenin indeksini döndürür.
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
public TableStyleElement get(int index)
```


Tablo stilinin bir öğesini indeksine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
### getByTableStyleElementType(int type) {#getByTableStyleElementType-int-}
```
public TableStyleElement getByTableStyleElementType(int type)
```


Tablo stilinin öğesini öğe tipine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [TableStyleElementType](../../com.aspose.cells/tablestyleelementtype). Öğenin tipi. |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement) - Returns [TableStyleElement](../../com.aspose.cells/tablestyleelement) object
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
### getTableStyleElementWithIndex(int index) {#getTableStyleElementWithIndex-int-}
```
public TableStyleElement getTableStyleElementWithIndex(int index)
```


Tablo stilinin bir öğesini indeksine göre alır.

**Remarks**

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen Aspose.Cells.Tables.TableStyleElementCollection.this[int index] özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
### getTableStyleElementWithType(int type) {#getTableStyleElementWithType-int-}
```
public TableStyleElement getTableStyleElementWithType(int type)
```


Tablo stilinin öğesini öğe tipine göre alır.

**Remarks**

NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen Aspense.Cells.Tables.TableStyleElementCollection.this[TableStyleElementType type] özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tip | int |  |

**Returns:**
[TableStyleElement](../../com.aspose.cells/tablestyleelement)
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

