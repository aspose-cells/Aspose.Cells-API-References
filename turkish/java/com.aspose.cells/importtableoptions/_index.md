---
title: "ImportTableOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Verilerin hücrelere içe aktarılması seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Verilerin hücrelere içe aktarılması seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Varsayılan içe aktarma seçeneklerini oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Veri kaynağından içe aktarılacak sütunları (0 tabanlı) alır. null, tüm sütunların içe aktarılacağı anlamına gelir. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Stil ızgara görünümünün hücrelere uygulanıp uygulanmayacağını gösterir. |
| [getConvertNumericData()](#getConvertNumericData--) | Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır. |
| [getDateFormat()](#getDateFormat--) | İçe aktarılan tarih saat değerlerine sahip hücreler için tarih biçimi dizesini alır. |
| [getDefaultValues()](#getDefaultValues--) | Tablodaki değer için varsayılan değer null'dır. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Başlığın alan adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [getInsertRows()](#getInsertRows--) | Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir. |
| [getNumberFormats()](#getNumberFormats--) | Sayı biçimlerini alır. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir. |
| [getStyles()](#getStyles--) | Tablonun her sütunu için stilleri alır. |
| [getTotalColumns()](#getTotalColumns--) | Veri kaynağından içe aktarılacak toplam sütun sayısını alır. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [getTotalRows()](#getTotalRows--) | Veri kaynağından içe aktarılacak toplam satır sayısını alır. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Alan adının içe aktarılıp aktarılmayacağını gösterir. |
| [isFormulas()](#isFormulas--) | Verilerin formül olup olmadığını gösterir. |
| [isHtmlString()](#isHtmlString--) | Değerin html etiketleri içerip içermediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Veri kaynağından içe aktarılacak sütunları (0 tabanlı) ayarlar. null, tüm sütunların içe aktarılması gerektiği anlamına gelir. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Stil ızgara görünümünün hücrelere uygulanıp uygulanmayacağını gösterir. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Dizge değerinin sayısal ya da tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesi ayarlar. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | Tablodaki değer için varsayılan değer null'dır. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Başlığın alan adı olarak dışa aktarılıp aktarılmayacağını gösterir. |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Alan adının içe aktarılıp aktarılmayacağını gösterir. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Verilerin formül olup olmadığını gösterir. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Değerin html etiketleri içerip içermediğini gösterir. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Sayı biçimlerini ayarlar |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Tablonun her sütunu için stilleri ayarlar. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Veri kaynağından içe aktarılacak toplam sütun sayısını ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [setTotalRows(int value)](#setTotalRows-int-) | Veri kaynağından içe aktarılacak toplam satır sayısını ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Varsayılan içe aktarma seçeneklerini oluşturur.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Veri kaynağından içe aktarılacak sütunları (0 tabanlı) alır. null, tüm sütunların içe aktarılacağı anlamına gelir.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Stil ızgara görünümünün hücrelere uygulanıp uygulanmayacağını gösterir.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Dize değerinin sayısal veya tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


İçe aktarılan tarih saat değerlerine sahip hücreler için tarih biçimi dizesini alır.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


Tablodaki değer için varsayılan değer null'dır.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Başlığın alan adı olarak dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca DataTable için çalışır.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Sayı biçimlerini alır.

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Tablonun her sütunu için stilleri alır.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Veri kaynağından içe aktarılacak toplam sütun sayısını alır. -1, verilen veri kaynağının tüm satırları anlamına gelir.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Veri kaynağından içe aktarılacak toplam satır sayısını alır. -1, verilen veri kaynağının tüm satırları anlamına gelir.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Alan adının içe aktarılıp aktarılmayacağını gösterir.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Verilerin formül olup olmadığını gösterir.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Değerin html etiketleri içerip içermediğini gösterir.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Birleştirilmiş hücrelerin kontrol edilip edilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Veri kaynağından içe aktarılacak sütunları (0 tabanlı) ayarlar. null, tüm sütunların içe aktarılması gerektiği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Stil ızgara görünümünün hücrelere uygulanıp uygulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Dizge değerinin sayısal ya da tarih değerine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


İçe aktarılan tarih‑zaman değerlerine sahip hücreler için tarih biçimi dizesi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


Tablodaki değer için varsayılan değer null'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Başlığın alan adı olarak dışa aktarılıp aktarılmayacağını gösterir.

**Remarks**

Yalnızca DataTable için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Alan adının içe aktarılıp aktarılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Verilerin formül olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Değerin html etiketleri içerip içermediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Veri kayıtlarını içe aktarmak için yeni satırların eklenip eklenmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Sayı biçimlerini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Satır eklerken ilk satırın aşağı kaydırılıp kaydırılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Tablonun her sütunu için stilleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Veri kaynağından içe aktarılacak toplam sütun sayısını ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Veri kaynağından içe aktarılacak toplam satır sayısını ayarlar. -1, verilen veri kaynağının tüm satırları anlamına gelir.

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

