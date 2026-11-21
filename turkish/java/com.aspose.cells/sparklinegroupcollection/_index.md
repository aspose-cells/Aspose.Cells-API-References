---
title: "SparklineGroupCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/sparklinegroupcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SparklineGroupCollection extends CollectionBase
```

Bir [SparklineGroup](../../com.aspose.cells/sparklinegroup) nesneleri koleksiyonunu kapsar.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, "A1:D1", false, ca);
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         book.save("output.xlsx", SaveFormat.XLSX);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int type)](#add-int-) | Koleksiyona bir [Sparkline](../../com.aspose.cells/sparkline) içeren bir [SparklineGroup](../../com.aspose.cells/sparklinegroup) ekler. |
| [add(int type, String dataRange, boolean isVertical, CellArea locationRange)](#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-) | Koleksiyona bazı [Sparkline](../../com.aspose.cells/sparkline) içeren bir [SparklineGroup](../../com.aspose.cells/sparklinegroup) ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [clearSparklineGroups(CellArea cellArea)](#clearSparklineGroups-com.aspose.cells.CellArea-) | Hücre alanıyla çakışan sparkline gruplarını temizler. |
| [clearSparklines(CellArea cellArea)](#clearSparklines-com.aspose.cells.CellArea-) | Hücre alanı içinde bulunan sparklineları temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [SparklineGroup](../../com.aspose.cells/sparklinegroup) öğesini alır. |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


Koleksiyona bir [Sparkline](../../com.aspose.cells/sparkline) içeren bir [SparklineGroup](../../com.aspose.cells/sparklinegroup) ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Sparkline grubunun türünü belirtir. |

**Returns:**
int - [SparklineGroup](../../com.aspose.cells/sparklinegroup) nesne indeksi.
### add(int type, String dataRange, boolean isVertical, CellArea locationRange) {#add-int-java.lang.String-boolean-com.aspose.cells.CellArea-}
```
public int add(int type, String dataRange, boolean isVertical, CellArea locationRange)
```


Koleksiyona bazı [Sparkline](../../com.aspose.cells/sparkline) içeren bir [SparklineGroup](../../com.aspose.cells/sparklinegroup) ekler.

**Remarks**

Bu yöntem aynı zamanda sparklineları oluşturur. Eğer  doğru ise, dataRange ve locationRange içindeki satır sayısı aynı olmalıdır. Eğer  yanlış ise, dataRange ve locationRange içindeki sütun sayısı aynı olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [SparklineType](../../com.aspose.cells/sparklinetype). Sparkline grubunun türünü belirtir. |
| dataRange | java.lang.String | Sparkline grubunun veri aralığını belirtir. |
| isVertical | boolean | Sparklineları veri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| locationRange | [CellArea](../../com.aspose.cells/cellarea) | Sparklineların yerleştirileceği konumu belirtir. |

**Returns:**
int - [SparklineGroup](../../com.aspose.cells/sparklinegroup) nesne indeksi.
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

### clearSparklineGroups(CellArea cellArea) {#clearSparklineGroups-com.aspose.cells.CellArea-}
```
public void clearSparklineGroups(CellArea cellArea)
```


Hücre alanıyla çakışan sparkline gruplarını temizler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Hücre alanını belirtir |

### clearSparklines(CellArea cellArea) {#clearSparklines-com.aspose.cells.CellArea-}
```
public void clearSparklines(CellArea cellArea)
```


Hücre alanı içinde bulunan sparklineları temizler.

**Remarks**

[SparklineGroup](../../com.aspose.cells/sparklinegroup) will be removed too if it does not contains any [Sparkline](../../com.aspose.cells/sparkline).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Hücre alanını belirtir |

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
public SparklineGroup get(int index)
```


Belirtilen indeksteki [SparklineGroup](../../com.aspose.cells/sparklinegroup) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[SparklineGroup](../../com.aspose.cells/sparklinegroup) - The element at the specified index.
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

