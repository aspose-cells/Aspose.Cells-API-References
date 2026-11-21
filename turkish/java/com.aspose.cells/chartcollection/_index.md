---
title: "ChartCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

Bir [Chart](../../com.aspose.cells/chart) nesnesi koleksiyonunu kapsar.

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Önceden ayarlanmış şablonla bir grafik ekler. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | Grafiği koleksiyona ekler. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Grafiği koleksiyona ekler. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Grafiği koleksiyona ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Grafiği koleksiyona ekler. |
| [clear()](#clear--) | Tüm grafikleri temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Chart](../../com.aspose.cells/chart) öğesini alır. |
| [get(String name)](#get-java.lang.String-) | Grafiği ada göre alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Belirli grafiği kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirli indeksteki bir grafiği kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Önceden ayarlanmış şablonla bir grafik ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | byte[] | Grafik şablonu dosyasının (.crtx) verileri. |
| dataRange | java.lang.String | Grafiğin veri aralığını belirtir. |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| rightRow | int | Alt sağ satır indeksi |
| bottomColumn | int | Alt sağ sütun indeksi |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) nesne indeksi.
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Grafiği koleksiyona ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Grafik türü |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) nesne indeksi.
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Grafiği koleksiyona ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Grafik türü |
| dataRange | java.lang.String | Grafiğin veri aralığını belirtir. |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| rightRow | int | Alt sağ satır indeksi |
| bottomColumn | int | Alt sağ sütun indeksi |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) nesne indeksi.
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Grafiği koleksiyona ekler.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\\#add-int-String-boolean-int-int-int-int-) özelliğini kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Grafik türü |
| dataRange | java.lang.String | Grafiğin veri aralığını belirtir. |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| rightRow | int | Alt sağ satır indeksi |
| bottomColumn | int | Alt sağ sütun indeksi |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) nesne indeksi.
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
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


Grafiği koleksiyona ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Grafik türü |
| sol | int | Köşeye x ofseti |
| üst | int | Köşeye y ofseti |
| genişlik | int | Grafik genişliği |
| yükseklik | int | Grafik yüksekliği |

**Returns:**
int - [Chart](../../com.aspose.cells/chart) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm grafikleri temizler.

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
public Chart get(int index)
```


Belirtilen indeksteki [Chart](../../com.aspose.cells/chart) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


Grafiği ada göre alır.

**Remarks**

Varsayılan grafik adı null'dır. Bu yüzden grafiğin adını açıkça ayarlamanız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Grafik adı. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
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




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


Belirli grafiği kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirli indeksteki bir grafiği kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Grafik indeksi. |

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

