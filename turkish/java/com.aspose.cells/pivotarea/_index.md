---
title: "PivotArea"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot tablo'nun seçili alanını sunar."
type: docs
url: /tr/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Pivot tablo'nun seçili alanını sunar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | PivotTable'ın seçilen alanını sunar. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Bu kuralın uygulandığı PivotTable bölgesini alır. |
| [getCellAreas()](#getCellAreas--) | Bu pivot alanının hücre alanlarını alır. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Bu PivotArea için tüm filtreleri alır. |
| [getOnlyData()](#getOnlyData--) | Yalnızca bir öğe seçimi için veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir. |
| [getOnlyLabel()](#getOnlyLabel--) | Yalnızca bir öğe seçimi için veri etiketlerinin seçilip seçilmediğini gösterir. |
| [getRuleType()](#getRuleType--) | Seçim kuralının tipini alır. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Sütun toplamının dahil edilip edilmediğini gösterir. |
| [isOutline()](#isOutline--) | Kuralın, taslak modunda olan bir alana referans verip vermediğini gösterir. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Satır toplamının dahil edilip edilmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Filtreli alanı seç. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Bölgede bir alanı alan olarak seç. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Bölgede bir alanı alan olarak seç. |
| [setAxisType(int value)](#setAxisType-int-) | Bu kuralın uygulandığı PivotTable bölgesini ayarlar. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Sütun toplamının dahil edilip edilmediğini gösterir. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Yalnızca bir öğe seçimi için veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Yalnızca bir öğe seçimi için veri etiketlerinin seçilip seçilmediğini gösterir. |
| [setOutline(boolean value)](#setOutline-boolean-) | Kuralın, taslak modunda olan bir alana referans verip vermediğini gösterir. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Satır toplamının dahil edilip edilmediğini gösterir. |
| [setRuleType(int value)](#setRuleType-int-) | Seçim kuralının tipini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


PivotTable'ın seçilen alanını sunar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Bu kuralın uygulandığı PivotTable bölgesini alır.

Bkz. [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Bu pivot alanının hücre alanlarını alır.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


Bu PivotArea için tüm filtreleri alır.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Yalnızca bir öğe seçimi için veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Yalnızca bir öğe seçimi için veri etiketlerinin seçilip seçilmediğini gösterir.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Seçim kuralının tipini alır.

Bakın [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


Sütun toplamının dahil edilip edilmediğini gösterir.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Kuralın, taslak modunda olan bir alana referans verip vermediğini gösterir.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Satır toplamının dahil edilip edilmediğini gösterir.

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


Filtreli alanı seç.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Bu kuralın uygulandığı PivotTable bölgesi. |
| fieldPosition | int | Bu kuralın uygulandığı eksen içindeki alanın konumu. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Yapısal bir seçim sırasında bir PivotTable'da neyin seçilebileceğini belirtir. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Bölgede bir alanı alan olarak seç.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Bölge türü. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Pivot alanı. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Bölgede bir alanı alan olarak seç.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Bölge türü. |
| fieldName | java.lang.String | Pivot alanının adı. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Bu kuralın uygulandığı PivotTable bölgesini ayarlar.

Bkz. [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Sütun toplamının dahil edilip edilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Yalnızca bir öğe seçimi için veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Yalnızca bir öğe seçimi için veri etiketlerinin seçilip seçilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Kuralın, taslak modunda olan bir alana referans verip vermediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Satır toplamının dahil edilip edilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Seçim kuralının tipini ayarlar.

Bakın [PivotAreaType](../../com.aspose.cells/pivotareatype).

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

