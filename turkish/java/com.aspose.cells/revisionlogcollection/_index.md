---
title: "RevisionLogCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm revizyon günlüklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/revisionlogcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class RevisionLogCollection extends CollectionBase
```

Tüm revizyon günlüklerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | İndeks ile [RevisionLog](../../com.aspose.cells/revisionlog) alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getDaysPreservingHistory()](#getDaysPreservingHistory--) | Elektronik tablo uygulamasının bu çalışma kitabı için değişiklik geçmişini tutacağı gün sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [highlightChanges(HighlightChangesOptions options)](#highlightChanges-com.aspose.cells.HighlightChangesOptions-) | Paylaşılan çalışma kitabındaki değişiklikleri vurgular. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [setDaysPreservingHistory(int value)](#setDaysPreservingHistory-int-) | Elektronik tablo uygulamasının bu çalışma kitabı için değişiklik geçmişini tutacağı gün sayısını ayarlar. |
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
public RevisionLog get(int index)
```


İndeks ile [RevisionLog](../../com.aspose.cells/revisionlog) alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[RevisionLog](../../com.aspose.cells/revisionlog) - Returns [RevisionLog](../../com.aspose.cells/revisionlog) object.
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
### getDaysPreservingHistory() {#getDaysPreservingHistory--}
```
public int getDaysPreservingHistory()
```


Elektronik tablo uygulamasının bu çalışma kitabı için değişiklik geçmişini tutacağı gün sayısını alır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### highlightChanges(HighlightChangesOptions options) {#highlightChanges-com.aspose.cells.HighlightChangesOptions-}
```
public void highlightChanges(HighlightChangesOptions options)
```


Paylaşılan çalışma kitabındaki değişiklikleri vurgular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [HighlightChangesOptions](../../com.aspose.cells/highlightchangesoptions) | Hangi değişikliklerin izleneceğini filtrelemek için seçenekleri ayarlar. |

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

### setDaysPreservingHistory(int value) {#setDaysPreservingHistory-int-}
```
public void setDaysPreservingHistory(int value)
```


Elektronik tablo uygulamasının bu çalışma kitabı için değişiklik geçmişini tutacağı gün sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

