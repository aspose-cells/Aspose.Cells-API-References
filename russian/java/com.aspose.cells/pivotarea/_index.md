---
title: "PivotArea"
second_title: "Справочник API Aspose.Cells for Java"
description: "Отображает выбранную область сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Отображает выбранную область сводной таблицы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Отображает выбранную область сводной таблицы. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Получает область сводной таблицы, к которой применяется это правило. |
| [getCellAreas()](#getCellAreas--) | Получает области ячеек этой области сводной таблицы. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Получает все фильтры для этой области сводной таблицы. |
| [getOnlyData()](#getOnlyData--) | Указывает, выбраны ли только значения данных (в области данных представления) для выбранного элемента и не включают ли метки элементов. |
| [getOnlyLabel()](#getOnlyLabel--) | Указывает, выбраны ли только метки данных для выбранного элемента. |
| [getRuleType()](#getRuleType--) | Получает тип правила выбора. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Указывает, включён ли общий итог по столбцу. |
| [isOutline()](#isOutline--) | Указывает, относится ли правило к области, находящейся в режиме структуры. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Указывает, включён ли общий итог по строке. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Выберите область с фильтрами. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Выберите поле в области в качестве области. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Выберите поле в области в качестве области. |
| [setAxisType(int value)](#setAxisType-int-) | Устанавливает область сводной таблицы, к которой применяется это правило. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Указывает, включён ли общий итог по столбцу. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Указывает, выбраны ли только значения данных (в области данных представления) для выбранного элемента и не включают ли метки элементов. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Указывает, выбраны ли только метки данных для выбранного элемента. |
| [setOutline(boolean value)](#setOutline-boolean-) | Указывает, относится ли правило к области, находящейся в режиме структуры. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Указывает, включён ли общий итог по строке. |
| [setRuleType(int value)](#setRuleType-int-) | Устанавливает тип правила выбора. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Отображает выбранную область сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Получает область сводной таблицы, к которой применяется это правило.

Смотрите [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Получает области ячеек этой области сводной таблицы.

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


Получает все фильтры для этой области сводной таблицы.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Указывает, выбраны ли только значения данных (в области данных представления) для выбранного элемента и не включают ли метки элементов.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Указывает, выбраны ли только метки данных для выбранного элемента.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Получает тип правила выбора.

Смотрите [PivotAreaType](../../com.aspose.cells/pivotareatype).

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


Указывает, включён ли общий итог по столбцу.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Указывает, относится ли правило к области, находящейся в режиме структуры.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Указывает, включён ли общий итог по строке.

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


Выберите область с фильтрами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Область PivotTable, к которой применяется это правило. |
| fieldPosition | int | Позиция поля по оси, к которой применяется это правило. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Указывает, что можно выбрать в PivotTable во время структурированного выбора. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Выберите поле в области в качестве области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Поле сводной таблицы. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Выберите поле в области в качестве области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области. |
| fieldName | java.lang.String | Имя поля сводной таблицы. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Устанавливает область сводной таблицы, к которой применяется это правило.

Смотрите [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Указывает, включён ли общий итог по столбцу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Указывает, выбраны ли только значения данных (в области данных представления) для выбранного элемента и не включают ли метки элементов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Указывает, выбраны ли только метки данных для выбранного элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Указывает, относится ли правило к области, находящейся в режиме структуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Указывает, включён ли общий итог по строке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Устанавливает тип правила выбора.

Смотрите [PivotAreaType](../../com.aspose.cells/pivotareatype).

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

