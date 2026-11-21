---
title: "PivotFilterCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm PivotFilter'ların bir koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Tüm PivotFilter'ların bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Belirli türe bir PivotFilter nesnesi ekler |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Satır veya sütun pivot alanının tarih ayarına göre filtreler. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Satır veya sütun pivot alanının başlıklarına göre filtreler. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Veri pivot alanının değerlerine göre filtreler. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Veri pivot alanının değerlerine göre filtreler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Belirli PivotField'dan PivotFilter'ı temizle |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirli indeksteki pivotfilter nesnesini alır. |
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
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Belirli türe bir PivotFilter nesnesi ekler

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() ve AddDateFilter() yöntemlerini kullanın. Bu yöntem Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | PivotField indeksi |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). PivotFilter türü |

**Returns:**
int - bu PivotFilterCollection içindeki PivotFilter nesnesinin indeksi.
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
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Satır veya sütun pivot alanının tarih ayarına göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | int | Kaynakta alanın indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Filtre koşulunun tarih etiketi |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Aralık filtre koşulunun üst sınır tarih etiketi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Satır veya sütun pivot alanının başlıklarına göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | int | Kaynakta alanın indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| label1 | java.lang.String | Filtre koşulunun etiketi |
| label2 | java.lang.String | Arasındaki filtre koşulunun üst sınır etiketi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Veri pivot alanının değerlerine göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | int | Kaynakta alanın indeksi. |
| valueFieldIndex | int | Veri bölgesindeki veri alanının indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. Yalnızca Count, Sum ve Percent olabilir. |
| isTop | boolean | Filtrenin üstten mi alttan mı olduğunu gösterir |
| itemCount | int | Öğe sayısı |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Veri pivot alanının değerlerine göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseFieldIndex | int | Kaynakta alanın indeksi. |
| valueFieldIndex | int | Değer bölgesindeki değer alanının indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| value1 | double | Filtre koşulunun değeri |
| value2 | double | Arasındaki filtre koşulunun üst sınır değeri |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


CollectionBase örneğinden tüm nesneleri kaldırır.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Belirli PivotField'dan PivotFilter'ı temizle

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | PivotField indeksi |

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
public PivotFilter get(int index)
```


Belirli indeksteki pivotfilter nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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

