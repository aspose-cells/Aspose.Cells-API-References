---
title: "CellWatchCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bu çalışma sayfasındaki izleme penceresinde izlenen hücrelerin koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/cellwatchcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CellWatchCollection extends CollectionBase
```

'watch window' içinde izlenen bu çalışma sayfasındaki hücre koleksiyonunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
         // Add Cell Watch Item into the watch window
         sheet.getCellWatches().add("B2");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CellWatchCollection()](#CellWatchCollection--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Bir satır ve sütun ile [CellWatch](../../com.aspose.cells/cellwatch) ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName)](#add-java.lang.String-) | Hücrenin adıyla [CellWatch](../../com.aspose.cells/cellwatch) ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | İndekse göre [CellWatch](../../com.aspose.cells/cellwatch) alır ve ayarlar. |
| [get(String cellName)](#get-java.lang.String-) | Hücre adıyla [CellWatch](../../com.aspose.cells/cellwatch) alır ve ayarlar. |
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
### CellWatchCollection() {#CellWatchCollection--}
```
public CellWatchCollection()
```


### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Bir satır ve sütun ile [CellWatch](../../com.aspose.cells/cellwatch) ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
int - Bu öğenin koleksiyondaki konumunu döndürür.
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


Hücrenin adıyla [CellWatch](../../com.aspose.cells/cellwatch) ekler.

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
public CellWatch get(int index)
```


İndekse göre [CellWatch](../../com.aspose.cells/cellwatch) alır ve ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
### get(String cellName) {#get-java.lang.String-}
```
public CellWatch get(String cellName)
```


Hücre adıyla [CellWatch](../../com.aspose.cells/cellwatch) alır ve ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücrenin adı. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
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

