---
title: "PivotFilter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет PivotFilter в коллекции PivotFilter."
type: docs
url: /ru/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Представляет PivotFilter в коллекции PivotFilter.

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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Получает автофильтр сводного фильтра. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Получает значения числового фильтра. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Получает порядок оценки сводного фильтра. |
| [getFieldIndex()](#getFieldIndex--) | Получает индекс исходного поля, к которому применяется этот сводный фильтр. |
| [getFilterCategory()](#getFilterCategory--) | Получает категорию этого фильтра. |
| [getFilterType()](#getFilterType--) | Получает тип фильтра сводного фильтра. |
| [getLabels()](#getLabels--) | Получает метки фильтра подписи. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Указывает индекс поля измерения куба. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Получает индекс поля измерения сводного фильтра. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Получает индекс поля свойства члена сводного фильтра. |
| [getName()](#getName--) | Получает имя сводного фильтра. |
| [getNumberValues()](#getNumberValues--) | Получает значения числового фильтра. |
| [getTop10Value()](#getTop10Value--) | Получает настройку Top 10 фильтра. |
| [getUseWholeDay()](#getUseWholeDay--) | Указывает, следует ли использовать полные дни в критериях фильтрации по дате. |
| [getValue1()](#getValue1--) | Получает строковое значение1 метки сводного фильтра. |
| [getValue2()](#getValue2--) | Получает строковое значение2 метки сводного фильтра. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Получает индекс поля значения в области значений. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Получает порядок оценки сводного фильтра. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Получает индекс поля измерения сводного фильтра. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Получает индекс поля свойства члена сводного фильтра. |
| [setName(String value)](#setName-java.lang.String-) | Получает имя сводного фильтра. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Указывает, следует ли использовать полные дни в критериях фильтрации по дате. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Получает строковое значение1 метки сводного фильтра. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Получает строковое значение2 метки сводного фильтра. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Получает индекс поля значения в области значений. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Получает автофильтр сводного фильтра.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод FilterLabel, FilterValue, FilterDate или FilterTop10. Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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


Получает значения числового фильтра.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Получает порядок оценки сводного фильтра.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Получает индекс исходного поля, к которому применяется этот сводный фильтр.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


Получает категорию этого фильтра.

См. [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Получает тип фильтра сводного фильтра.

Смотрите [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


Получает метки фильтра подписи.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


Указывает индекс поля куба измерения. Это свойство используется только фильтрами в OLAP‑сводных таблицах и определяет, к какому измерению следует применять фильтр значений.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Получает индекс поля измерения сводного фильтра.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotFilter.ValueFieldIndex. Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Получает индекс поля свойства члена сводного фильтра.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя сводного фильтра.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


Получает значения числового фильтра.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


Получает настройку Top 10 фильтра.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


Указывает, следует ли использовать полные дни в критериях фильтрации по дате.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


Получает строковое значение1 метки сводного фильтра.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Получает строковое значение2 метки сводного фильтра.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


Получает индекс поля значения в области значений.

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


Получает порядок оценки сводного фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


Получает индекс поля измерения сводного фильтра.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotFilter.ValueFieldIndex. Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


Получает индекс поля свойства члена сводного фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Получает имя сводного фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


Указывает, следует ли использовать полные дни в критериях фильтрации по дате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


Получает строковое значение1 метки сводного фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


Получает строковое значение2 метки сводного фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


Получает индекс поля значения в области значений.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

