---
title: "AutoFilter"
second_title: "Aspose.Cells for Java API Referansı"
description: "Temsil eder belirtilen çalışma sayfası için otomatik filtrelemeyi."
type: docs
url: /tr/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Temsil eder belirtilen çalışma sayfası için otomatik filtrelemeyi.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Bir tarih filtresi ekler. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Bir doldurma rengi filtresi ekler. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Bir filtre sütunu için filtre ekler. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Bir yazı tipi rengi filtresi ekler. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Bir simge filtresi ekler. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Bir listeyi özel bir ölçüte göre filtreler. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Bir listeyi özel ölçütlerle filtreler. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Dinamik bir filtre ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Bir listeyi belirtilen ölçütlerle filtreler. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Listedeki ilk 10 öğeyi filtrele |
| [getCellArea()](#getCellArea--) | Bu AutoFilter'ın uygulandığı [CellArea](../../com.aspose.cells/cellarea) öğesini alır. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Belirtilen AutoFilter'ın uygulandığı [CellArea](../../com.aspose.cells/cellarea) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Filtre sütunlarının koleksiyonunu alır. |
| [getRange()](#getRange--) | Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder. |
| [getShowFilterButton()](#getShowFilterButton--) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [getSorter()](#getSorter--) | Veri sıralayıcısını alır. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Listedeki tüm boş hücreleri eşleştir. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Listedeki tüm boş olmayan hücreleri eşleştir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Satırları gizlemek veya göstermek için otomatik filtreleri yenile. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Tüm gizli satırların indekslerini alır. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Bir tarih filtresini kaldırır. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Belirli bir filtreyi kaldırır. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Bir filtre sütunu için filtreyi kaldırır. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar. |
| [setRange(String value)](#setRange-java.lang.String-) | Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [showAll()](#showAll--) | Tüm satırların gizlenmesini kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Bir tarih filtresi ekler.

**Remarks**

Eğer DateTimeGroupingType Yıl ise, yalnızca yıl parametresi etkilenir. Eğer DateTiemGroupingType Ay ise, yalnızca yıl ve ay parametreleri etkilenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Gruplama türü |
| yıl | int | Yıl. |
| ay | int | Ay. |
| gün | int | Gün. |
| saat | int | Saat. |
| dakika | int | Dakika. |
| saniye | int | Saniye. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Bir doldurma rengi filtresi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Arka plan desen türü. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Ön plan rengi. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Arka plan rengi. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Bir filtre sütunu için filtre ekler.

**Remarks**

MS Excel 2007, bir filtre sütununda birden çok seçim desteği sağlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| kriter | java.lang.String | Belirtilen kriter (bir dize; örneğin, "101"). Sadece null olabilir veya bu sütundaki hücrelerin değerlerinden biri olabilir. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Bir yazı tipi rengi filtresi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | Bu [CellsColor](../../com.aspose.cells/cellscolor) nesnesi. |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Bir simge filtresi ekler.

**Remarks**

Yalnızca simge filtresi eklemeyi destekler. Filtre simge filtresi ise hangi satırın görünür olduğunu kontrol etmeyi desteklemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Simge seti türü. |
| iconId | int | Simge kimliği. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Bir listeyi özel bir ölçüte göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filtre operatör türü |
| criteria1 | java.lang.Object | Özel kriter |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Bir listeyi özel ölçütlerle filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filtre operatör türü |
| criteria1 | java.lang.Object | Özel kriter |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filtre operatör türü |
| criteria2 | java.lang.Object | Özel kriter |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Dinamik bir filtre ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Dinamik filtre türü. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Bir listeyi belirtilen ölçütlerle filtreler.

**Remarks**

Aspose.Cells bu alandaki diğer tüm filtre ayarlarını MS Excel 97-2003 gibi kaldıracaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| kriter | java.lang.String | Belirtilen kriter (bir dize; örneğin, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Listedeki ilk 10 öğeyi filtrele

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| isTop | boolean | Filtrenin üstten mi alttan mı olduğunu gösterir |
| isPercent | boolean | Öğelerin yüzde mi yoksa sayı mı olduğunu gösterir. |
| itemCount | int | Öğe sayısı |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Bu AutoFilter'ın uygulandığı [CellArea](../../com.aspose.cells/cellarea) öğesini alır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Belirtilen AutoFilter'ın uygulandığı [CellArea](../../com.aspose.cells/cellarea) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| refreshAppliedRange | boolean | Uygulanan aralığın yenilenip yenilenmeyeceği. Otomatik filtrenin uygulanan aralığı için, hücre verileri değiştiğinde son satır değişebilir. Bu bayrak true ise, aralığın son satırı mevcut hücre verilerine göre yeniden hesaplanacaktır. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Filtre sütunlarının koleksiyonunu alır.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Veri sıralayıcısını alır.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Listedeki tüm boş hücreleri eşleştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Listedeki tüm boş olmayan hücreleri eşleştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Satırları gizlemek veya göstermek için otomatik filtreleri yenile.

**Returns:**
int[] - Tüm gizli satırların dizinlerini döndürür.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Tüm gizli satırların indekslerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hideRows | boolean | True ise, filtrelenmiş satırları gizle. |

**Returns:**
int[] - Tüm gizli satır dizinlerini döndürür.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Bir tarih filtresini kaldırır.

**Remarks**

Eğer DateTimeGroupingType Yıl ise, yalnızca yıl parametresi etkilenir. Eğer DateTiemGroupingType Ay ise, yalnızca yıl ve ay parametreleri etkilenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Gruplama türü |
| yıl | int | Yıl. |
| ay | int | Ay. |
| gün | int | Gün. |
| saat | int | Saat. |
| dakika | int | Dakika. |
| saniye | int | Saniye. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Belirli bir filtreyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Belirli filtre indeksi |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Bir filtre sütunu için filtreyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | int | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan alan 0'dır). |
| kriter | java.lang.String | Belirtilen kriter (bir dize; örneğin, "101"). Sadece null olabilir veya bu sütundaki hücrelerin değerlerinden biri olabilir. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Son sütun indeksi. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Tüm satırların gizlenmesini kaldır.

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

