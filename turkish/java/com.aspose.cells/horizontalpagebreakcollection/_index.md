---
title: "HorizontalPageBreakCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) nesnelerinden oluşan bir koleksiyonu kapsüller.

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int row)](#add-int-) | Koleksiyona bir yatay sayfa sonu ekler. |
| [add(int row, int column)](#add-int-int-) | Koleksiyona bir yatay sayfa sonu ekler. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Koleksiyona bir yatay sayfa sonu ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName)](#add-java.lang.String-) | Koleksiyona bir yatay sayfa sonu ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) öğesini alır. |
| [get(String cellName)](#get-java.lang.String-) | Belirtilen hücre adıyla [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen isimdeki HPageBreak öğesini kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Koleksiyona bir yatay sayfa sonu ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücre satır indeksi, sıfır tabanlı. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) nesne indeksi.
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Koleksiyona bir yatay sayfa sonu ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücre satır indeksi, sıfır tabanlı. |
| sütun | int | Hücre sütun indeksi, sıfır tabanlı. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) nesne indeksi.
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Koleksiyona bir yatay sayfa sonu ekler.

**Remarks**

Bu yöntem, bir baskı alanı içinde yatay sayfa sonu eklemek için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi, sıfır tabanlı. |
| startColumn | int | Başlangıç sütun indeksi, sıfır tabanlı. |
| endColumn | int | Bitiş sütun indeksi, sıfır tabanlı. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) nesne indeksi.
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


Koleksiyona bir yatay sayfa sonu ekler.

**Remarks**

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

**Returns:**
int - [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) nesne indeksi.
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
public HorizontalPageBreak get(int index)
```


Belirtilen indeksteki [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Belirtilen hücre adıyla [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


Belirtilen isimdeki HPageBreak öğesini kaldırır.

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

