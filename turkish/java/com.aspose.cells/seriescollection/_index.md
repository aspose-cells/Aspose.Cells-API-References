---
title: "SeriesCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

Bir [Series](../../com.aspose.cells/series) nesneleri koleksiyonunu kapsar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | [Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | [Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | [Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler. |
| [changeColors(int type)](#changeColors-int-) | Çizelge serileri için Tek Renkli Palet ayarlar. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | İki serinin sırasını doğrudan değiştirir. |
| [clear()](#clear--) | Koleksiyonu temizler |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Series](../../com.aspose.cells/series) öğesini alır. |
| [getCategoryData()](#getCategoryData--) | Kategori ekseni değerlerinin aralığını alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getSecondCategoryData()](#getSecondCategoryData--) | İkinci kategori ekseni değerlerinin aralığını alır. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | Sıraya göre [Series](../../com.aspose.cells/series) öğesini alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [isColorVaried()](#isColorVaried--) | Nokta renklerinin değişken olup olmadığını temsil eder. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirli bir indeksteki seriyi kaldırır. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | Kategori ekseni değerlerinin aralığını ayarlar. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Nokta renklerinin değişken olup olmadığını temsil eder. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | İkinci kategori ekseni değerlerinin aralığını ayarlar. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | Grafikteki tüm serilerin adlarını ayarlar. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | İki serinin sırasını doğrudan değiştirir. |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


[Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler.

**Remarks**


Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üstüste kullanın.Örneğin, $C$2:$C$5.

Ardışık olmayan hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın.Örneğin: ($C$2,$D$5).

Bu yöntem yalnızca veri aralığı olarak basitçe işler. Akıllıca ChartCollection.Add() yöntemini kontrol etmek istiyorsanız.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataArea | java.lang.String | Veri serisini çizmek için kullanılacak değerleri belirtir |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. Doğruysa, [Series](../../com.aspose.cells/series) sütun sütun eklenecektir. |

**Returns:**
int - Eklenen ASeries'in NSeries içindeki ilk dizinini döndürür.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


[Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler.

**Remarks**


Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üstüste kullanın. Örneğin, $C$2:$C$5.

Ardışık olmayan hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin, ($C$2,$D$5).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | java.lang.String | Veri serisini çizmek için kullanılacak değerleri belirtir |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| checkLabels | boolean | Aralığın serinin adını içerip içermediğini gösterir |

**Returns:**
int - Eklenen ASeries'in NSeries içindeki ilk dizinini döndürür.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


[Series](../../com.aspose.cells/series) koleksiyonunu bir çizelgeye ekler.

**Remarks**


Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üstüste kullanın. Örneğin, R[1]C[1]:R[3]C[2].

Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin,(R[1]C[1],R[3]C[2]).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | java.lang.String | Veri serisini çizmek için kullanılacak değerleri belirtir |
| isVertical | boolean | Serileri hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |

**Returns:**
int - Eklenen ASeries'in NSeries içindeki ilk dizinini döndürür.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


Çizelge serileri için Tek Renkli Palet ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). Monokromatik Tür. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


İki serinin sırasını doğrudan değiştirir.

**Remarks**

NOT: Bu yöntem artık eski. Bunun yerine lütfen SeriesCollection.SwapSeries yöntemini kullanın. Bu yöntem, Haziran 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | int | Geçerli dizin |
| destIndex | int | Hedef dizin |

### clear() {#clear--}
```
public void clear()
```


Koleksiyonu temizler

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
public Series get(int index)
```


Belirtilen indeksteki [Series](../../com.aspose.cells/series) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


Kategori eksen değerlerinin aralığını alır. Hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "\\{2,6,8,10\\}") olabilir.

**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


İkinci kategori eksen değerlerinin aralığını alır. Hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "\\{2,6,8,10\\}") olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


Sıraya göre [Series](../../com.aspose.cells/series) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| order | int | Serilerin sırası |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Nokta renklerinin değişken olup olmadığını temsil eder.

**Remarks**

Yalnızca pasta grafiği için veya yalnızca bir seri olduğunda çalışır.

**Returns:**
boolean
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


Belirli bir indeksteki seriyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


Kategori eksen değerlerinin aralığını ayarlar. Hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "\{2,6,8,10\}") olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Nokta renklerinin değişken olup olmadığını temsil eder.

**Remarks**

Yalnızca pasta grafiği için veya yalnızca bir seri olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


İkinci kategori eksen değerlerinin aralığını ayarlar. Hücre aralığı (örneğin "d1:e10"), veya değer dizisi (örneğin "\{2,6,8,10\}") olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


Grafikteki tüm serilerin adlarını ayarlar.

**Remarks**


Başlangıç indeksi seri sayısından büyükse, geri dönecek ve hiçbir şey yapmayacaktır.

Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üstüste kullanın. Örneğin, $C$2:$C$5.

Ardışık hücrelerde veri ayarlanıyorsa, virgül ile ayırın. Örneğin, ($C$2,$D$5).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Adını ayarlamak istediğiniz ilk serinin indeksi. |
| area | java.lang.String | Seri adı için alanı belirtir. |
| isVertical | boolean | >Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


İki serinin sırasını doğrudan değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | int | Geçerli dizin |
| destIndex | int | Hedef dizin |

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

