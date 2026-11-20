---
title: "PivotTableCalculateOption"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры расчёта данных сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

Представляет параметры расчёта данных сводной таблицы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | Указывает, обновляются ли диаграммы на основе этой сводной таблицы. |
| [getRefreshData()](#getRefreshData--) | Указывает, обновляется ли источник данных сводной таблицы. |
| [getRefreshOption()](#getRefreshOption--) | Получает параметры обновления источника данных в кэш сводных таблиц. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Представляет способ резервирования отсутствующих элементов сводной таблицы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | Указывает, обновляются ли диаграммы на основе этой сводной таблицы. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | Указывает, обновляется ли источник данных сводной таблицы. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | Устанавливает параметры обновления источника данных в кэш сводных таблиц. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Представляет способ резервирования отсутствующих элементов сводной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


Указывает, обновляются ли диаграммы на основе этой сводной таблицы.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


Указывает, обновляется ли источник данных сводной таблицы.

**Remarks**

Если значение true, обновляет кэш сводных таблиц из источника данных, затем вычисляет все сводные таблицы на основе того же кэша.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


Получает параметры обновления источника данных в кэш сводных таблиц.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Представляет способ резервирования отсутствующих элементов сводной таблицы.

Смотрите [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Работает только когда [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) возвращает true.

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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


Указывает, обновляются ли диаграммы на основе этой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


Указывает, обновляется ли источник данных сводной таблицы.

**Remarks**

Если значение true, обновляет кэш сводных таблиц из источника данных, затем вычисляет все сводные таблицы на основе того же кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


Устанавливает параметры обновления источника данных в кэш сводных таблиц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Представляет способ резервирования отсутствующих элементов сводной таблицы.

Смотрите [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Работает только когда [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) возвращает true.

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

