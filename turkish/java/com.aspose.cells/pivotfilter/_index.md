---
title: "PivotFilter"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotFilter Koleksiyonu içinde bir PivotFilter'ı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

PivotFilter Koleksiyonu içinde bir PivotFilter'ı temsil eder.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Add top 10 filter
          pivot.getBaseFields().get(0).filterTop10(0, PivotFilterType.COUNT,false,2);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Pivot filtresinin otomatik filtresini alır. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Sayı filtresinin değerlerini alır. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Pivot filtresinin Değerlendirme Sırasını alır. |
| [getFieldIndex()](#getFieldIndex--) | Bu pivot filtrenin uygulandığı kaynak alanın dizinini alır. |
| [getFilterCategory()](#getFilterCategory--) | Bu filtrenin kategorisini alır. |
| [getFilterType()](#getFilterType--) | Pivot filtresinin filtre tipini alır. |
| [getLabels()](#getLabels--) | Başlık filtresinin etiketlerini alır. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Ölçüm küp alanının dizinini belirtir. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Pivot filtresinin ölçüm alanı dizinini alır. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Pivot filtresinin üye özelliği alanı dizinini alır. |
| [getName()](#getName--) | Pivot filtresinin adını alır. |
| [getNumberValues()](#getNumberValues--) | Sayı filtresinin değerlerini alır. |
| [getTop10Value()](#getTop10Value--) | Filtrenin ilk 10 ayarını alır. |
| [getUseWholeDay()](#getUseWholeDay--) | Tarih filtreleme kriterlerinde tam günlerin kullanılıp kullanılmayacağını gösterir. |
| [getValue1()](#getValue1--) | Etiket pivot filtresinin string değer1'ini alır. |
| [getValue2()](#getValue2--) | Etiket pivot filtresinin string değer2'sini alır. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Değer bölgesindeki değer alanının dizinini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Pivot filtresinin Değerlendirme Sırasını alır. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Pivot filtresinin ölçüm alanı dizinini alır. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Pivot filtresinin üye özelliği alanı dizinini alır. |
| [setName(String value)](#setName-java.lang.String-) | Pivot filtresinin adını alır. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Tarih filtreleme kriterlerinde tam günlerin kullanılıp kullanılmayacağını gösterir. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Etiket pivot filtresinin string değer1'ini alır. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Etiket pivot filtresinin string değer2'sini alır. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Değer bölgesindeki değer alanının dizinini alır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Pivot filtresinin otomatik filtresini alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen FilterLabel, FilterValue, FilterDate veya FilterTop10 yöntemini kullanın. Bu yöntem Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValues() {#getDateTimeValues--}
```
public DateTime[] getDateTimeValues()
```


Sayı filtresinin değerlerini alır.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Pivot filtresinin Değerlendirme Sırasını alır.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Bu pivot filtrenin uygulandığı kaynak alanın dizinini alır.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Bu filtrenin kategorisini alır.

Bakınız [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Pivot filtresinin filtre tipini alır.

Bakın [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Başlık filtresinin etiketlerini alır.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Ölçü küp alanının dizinini belirtir. Bu özellik yalnızca OLAP pivotlarındaki filtreler tarafından kullanılır ve değer filtresinin hangi ölçüde uygulanacağını belirtir.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Pivot filtresinin ölçüm alanı dizinini alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotFilter.ValueFieldIndex özelliğini kullanın. Bu yöntem Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Pivot filtresinin üye özelliği alanı dizinini alır.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Pivot filtresinin adını alır.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Sayı filtresinin değerlerini alır.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Filtrenin ilk 10 ayarını alır.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Tarih filtreleme kriterlerinde tam günlerin kullanılıp kullanılmayacağını gösterir.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Etiket pivot filtresinin string değer1'ini alır.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Etiket pivot filtresinin string değer2'sini alır.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Değer bölgesindeki değer alanının dizinini alır.

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




### setEvaluationOrder(int value) {#setEvaluationOrder-int-}
```
public void setEvaluationOrder(int value)
```


Pivot filtresinin Değerlendirme Sırasını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Pivot filtresinin ölçüm alanı dizinini alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotFilter.ValueFieldIndex özelliğini kullanın. Bu yöntem Kasım 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Pivot filtresinin üye özelliği alanı dizinini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Pivot filtresinin adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Tarih filtreleme kriterlerinde tam günlerin kullanılıp kullanılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Etiket pivot filtresinin string değer1'ini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Etiket pivot filtresinin string değer2'sini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Değer bölgesindeki değer alanının dizinini alır.

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

