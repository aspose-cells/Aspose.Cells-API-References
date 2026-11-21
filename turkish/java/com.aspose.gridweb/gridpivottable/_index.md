---
title: "GridPivotTable"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfasındaki PivotTable raporunu temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Bir çalışma sayfasındaki PivotTable raporunu temsil eder. PivotTable nesnesi, [GridPivotTable](../../com.aspose.gridweb/gridpivottable) koleksiyonunun bir üyesidir. PivotTables koleksiyonu, bir kontrol üzerindeki tüm PivotTable nesnelerini içerir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Alanı belirli alana ekler. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Alanı belirli alana ekler. |
| [calculateData()](#calculateData--) | PivotTable verilerini hücrelere hesaplar. |
| [clearAllFields()](#clearAllFields--) | tüm pivot alanlarını temizle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Alan türüne göre belirli alanları alır. |
| [fields(String fieldName)](#fields-java.lang.String-) | Alan adını kullanarak belirli alanı alır. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | PivotTable verilerini ve ayarlarını veri kaynağından yeniler. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Alanı belirli alana ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Alan bölgesi türü. |
| baseFieldIndex | int | Temel alanlardaki alan dizini. |

**Returns:**
int - Belirli alanlardaki alan konumu.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Alanı belirli alana ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Alan bölgesi türü. |
| fieldName | java.lang.String | Temel alanlardaki ad. |

**Returns:**
int - Belirli alanlardaki alan konumu. Eğer böyle bir alan yoksa, -1 döndür.
### calculateData() {#calculateData--}
```
public void calculateData()
```


PivotTable verilerini hücrelere hesaplar.

**Remarks**

Pivot aralığındaki Cell.Value, yöntem çağrılmadıysa doğru sonucu döndüremez. Bu yöntem, orijinal veri kaynağı yerine iç bir pivot önbelleğiyle verileri hesaplar. Bu nedenle veri kaynağı değiştirildiyse, lütfen önce RefreshData() yöntemini çağırın.

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


tüm pivot alanlarını temizle.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Alan türüne göre belirli alanları alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). alan türü. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Alan adını kullanarak belirli alanı alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldName | java.lang.String | alan adı. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshData() {#refreshData--}
```
public void refreshData()
```


PivotTable verilerini ve ayarlarını veri kaynağından yeniler.

**Remarks**

Verileri veri kaynağından bir pivot önbelleğine toplayacağız, ardından önbellekteki verileri hücrelere hesaplayacağız. Bu yöntem yalnızca tüm verileri bir pivot önbelleğine toplamak için kullanılır.

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

