---
title: "ExportTableOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm dışa aktarım tablo seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Tüm dışa aktarım tablo seçeneklerini temsil eder.

**Remarks**

Dışa aktarma ile ilgili bazı özel gereksinimler, örneğin hata değerlerini yok sayma gibi, varsa kullanıcı bu sınıfı genişleterek ilgili API'leri geçersiz kılarak hedefe ulaşabilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Bu değer, bu tabloda DBNull'ların izin verilip verilmediğini gösterir. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Hücrelerin HTML dize değerini DataTable'a dışa aktarır. |
| [getExportAsString()](#getExportAsString--) | Hücrelerin dize değerini DataTable'a dışa aktarır. |
| [getExportColumnName()](#getExportColumnName--) | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [getFormatStrategy()](#getFormatStrategy--) | Değeri dize olarak dışa aktarırken kullanılan biçim stratejisini alır. |
| [getIndexes()](#getIndexes--) | Dışa aktarılması gereken sütunların/satırların indeksleri. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Yalnızca görünen hücreleri dışa aktarır. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Yalnızca görünen sütunları dışa aktarır. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Yalnızca görünen satırları dışa aktarır. |
| [getRenameStrategy()](#getRenameStrategy--) | Sütunların yinelenen adları için strateji. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Dışa aktarılacak mevcut hücrenin değerini ön işleme tabi tut. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Bu değer, bu tabloda DBNull'ların izin verilip verilmediğini gösterir. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Hücrelerin HTML dize değerini DataTable'a dışa aktarır. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Hücrelerin dize değerini DataTable'a dışa aktarır. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Değeri string olarak dışa aktarırken format stratejisini ayarlar. |
| [setIndexes(int[] value)](#setIndexes-int---) | Dışa aktarılması gereken sütunların/satırların indeksleri. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Yalnızca görünen hücreleri dışa aktarır. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Yalnızca görünen sütunları dışa aktarır. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Yalnızca görünen satırları dışa aktarır. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Sütunların yinelenen adları için strateji. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. |
| [setVertical(boolean value)](#setVertical-boolean-) | Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Bu değer, bu tabloda DBNull'ların izin verilip verilmediğini gösterir.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. True, Aspose.Cells DataColumn'un tipini ayarlamadan önce sütundaki değer tiplerinin karışık olup olmadığını kontrol eder ve değer tipleri karışık ise DataColumn'un tipi string olur.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


Hücrelerin HTML dize değerini DataTable'a dışa aktarır.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Hücrelerin dize değerini DataTable'a dışa aktarır.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Değeri dize olarak dışa aktarırken kullanılan biçim stratejisini alır.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Varsayılan değer [CellValueFormatStrategy.CELL\\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Dışa aktarılması gereken sütunların/satırların indeksleri.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Yalnızca görünen hücreleri dışa aktarır.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Yalnızca görünen sütunları dışa aktarır.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Yalnızca görünen satırları dışa aktarır.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Sütunların yinelenen adları için strateji.

Bakınız [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. Örneğin, sütun tipi decimal ise ve değer decimal.MaxValue'dan büyük ve bu özellik true ise, tekrar istisna fırlatmayacağız. Varsayılan değer false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. Workbook dosyasındaki bir sütun DataTable'da bir satırı temsil ediyorsa false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


Dışa aktarılacak mevcut hücrenin değerini ön işleme tabi tut.

**Remarks**

Satır ve sütun indeksi, hücrenin çalışma sayfasındaki mutlak indeksidir, dışa aktarılan tablodaki indeks değildir. Kullanıcı, bu yöntemin geçersiz kılma uygulamasında mevcut hücrenin değerini kontrol edebilir; eğer mevcut hücre başka bir tip ve değerle değiştirilmesi gerekiyorsa, burada uygulanacak kod beklenen tip ve değeri CellValue nesnesine ayarlamalı ve true döndürmelidir. Varsayılan olarak bu yöntem hiçbir şey yapmaz ve false döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellRow | int | mevcut hücrenin satır indeksi |
| cellColumn | int | hücrenin sütun indeksi |
| value | [CellValue](../../com.aspose.cells/cellvalue) | mevcut hücrenin değeri ve tipi |

**Returns:**
boolean - Mevcut hücrenin farklı tip ve/veya değerle değiştirilip değiştirilmediği.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Bu değer, bu tabloda DBNull'ların izin verilip verilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


False, Aspose.Cells performans için DataColumn'un tipini ilk satırın değer tipine göre ayarlar. True, Aspose.Cells DataColumn'un tipini ayarlamadan önce sütundaki değer tiplerinin karışık olup olmadığını kontrol eder ve değer tipleri karışık ise DataColumn'un tipi string olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Hücrelerin HTML dize değerini DataTable'a dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Hücrelerin dize değerini DataTable'a dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Değeri string olarak dışa aktarırken format stratejisini ayarlar.

Bakınız [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Varsayılan değer [CellValueFormatStrategy.CELL\\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\\#CELL-STYLE).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Dışa aktarılması gereken sütunların/satırların indeksleri.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Yalnızca görünen hücreleri dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Yalnızca görünen sütunları dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Yalnızca görünen satırları dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Sütunların yinelenen adları için strateji.

Bakınız [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Sütun için geçersiz değerin atlanıp atlanmayacağını gösterir. Örneğin, sütun tipi decimal ise ve değer decimal.MaxValue'dan büyük ve bu özellik true ise, tekrar istisna fırlatmayacağız. Varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


Workbook dosyasındaki bir satır DataTable'da bir satırı temsil ediyorsa true. Workbook dosyasındaki bir sütun DataTable'da bir satırı temsil ediyorsa false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

