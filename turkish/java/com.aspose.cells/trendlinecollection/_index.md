---
title: "TrendlineCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Belirtilen veri serisi için tüm nesnelerin bir koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/trendlinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TrendlineCollection extends CollectionBase
```

Belirtilen veri serisi için tüm [Trendline](../../com.aspose.cells/trendline) nesnelerinin bir koleksiyonunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         worksheet.getCells().get("A1").putValue(50);
         worksheet.getCells().get("A2").putValue(100);
         worksheet.getCells().get("A3").putValue(150);
         worksheet.getCells().get("A4").putValue(200);
         worksheet.getCells().get("B1").putValue(60);
         worksheet.getCells().get("B2").putValue(32);
         worksheet.getCells().get("B3").putValue(50);
         worksheet.getCells().get("B4").putValue(40);
 
         //Adding a chart to the worksheet
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 3, 3, 15, 10);
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:a3", true);
         chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR, "MyTrendLine");
         Trendline line = chart.getNSeries().get(0).getTrendLines().get(0);
         line.setDisplayEquation(true);
         line.setDisplayRSquared(true);
         line.setColor(Color.getRed());
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int type)](#add-int-) | Bu koleksiyona belirtilen türde bir [Trendline](../../com.aspose.cells/trendline) nesnesi ekler. |
| [add(int type, String name)](#add-int-java.lang.String-) | Bu koleksiyona belirtilen tür ve ad ile bir [Trendline](../../com.aspose.cells/trendline) nesnesi ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Bir [Trendline](../../com.aspose.cells/trendline) nesnesini indeksine göre alır. |
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


Bu koleksiyona belirtilen türde bir [Trendline](../../com.aspose.cells/trendline) nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). Trendline türü. |

**Returns:**
int - [Trendline](../../com.aspose.cells/trendline) nesne indeksi.
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Bu koleksiyona belirtilen tür ve ad ile bir [Trendline](../../com.aspose.cells/trendline) nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). Trendline türü. |
| ad | java.lang.String | Trendline adı. |

**Returns:**
int - [Trendline](../../com.aspose.cells/trendline) nesne indeksi.
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
public Trendline get(int index)
```


Bir [Trendline](../../com.aspose.cells/trendline) nesnesini indeksine göre alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[Trendline](../../com.aspose.cells/trendline)
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

