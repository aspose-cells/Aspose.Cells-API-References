---
title: "PivotFormatCondition"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotFormatCondition Koleksiyonu içinde bir PivotTable Format Koşulunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

PivotFormatCondition Koleksiyonu içinde bir PivotTable Format Koşulunu temsil eder.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat) sınıfını kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Sütun alanlarında PivotTable koşullu biçim sınırını ekler. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Sütun alanlarında PivotTable koşullu biçim sınırını ekler. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Veri alanlarında PivotTable koşullu biçim sınırını ekler. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Veri alanlarında PivotTable koşullu biçim sınırını ekler. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Satır alanlarında PivotTable koşullu biçim sınırını ekler. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Satır alanlarında PivotTable koşullu biçim sınırını ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Özet tablo koşullu biçimi için koşulları al. |
| [getRuleType()](#getRuleType--) | Özet tablo koşul biçimi için kural tipini alır. |
| [getScopeType()](#getScopeType--) | Özet tablo koşullu biçimi için kapsam tipini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | PivotFormatCondition nesnesinin koşullu alanlarını ayarlar. |
| [setRuleType(int value)](#setRuleType-int-) | Özet tablo koşul biçimi için kural tipini ayarlar. |
| [setScopeType(int value)](#setScopeType-int-) | Özet tablo koşullu biçimi için kapsam tipini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Sütun alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | Sütun alanlarındaki PivotField. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Sütun alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField'ın adı. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Veri alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | Veri alanlarındaki PivotField. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Veri alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField'ın adı. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Satır alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | Satır alanlarındaki PivotField. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Satır alanlarında PivotTable koşullu biçim sınırını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField'ın adı. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Özet tablo koşullu biçimi için koşulları al.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Özet tablo koşul biçimi için kural tipini alır.

Bak [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Özet tablo koşullu biçimi için kapsam tipini alır.

Bak [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Returns:**
int
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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


PivotFormatCondition nesnesinin koşullu alanlarını ayarlar.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Özet tablo koşul biçimi için kural tipini ayarlar.

Bak [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Özet tablo koşullu biçimi için kapsam tipini ayarlar.

Bak [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

