---
title: "PivotCache"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет кэш памяти для некоторых отчетов сводных таблиц."
type: docs
url: /ru/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Представляет кэш памяти для некоторых отчетов сводных таблиц.

**Remarks**

Все данные будут собраны в этом кэше, и сводная таблица будет получать данные только из этого кэша, а не напрямую обращаться к источнику данных. Если источник данных некоторых [PivotTable](../../com.aspose.cells/pivottable)s одинаковый, они будут использовать один кэш.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [dispose()](#dispose--) | Освободить все ресурсы. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Получает количество неиспользуемых элементов, допускаемых до их удаления. |
| [getPivotTables()](#getPivotTables--) | Получает все сводные таблицы, использующие этот pivot cache. |
| [getSourceType()](#getSourceType--) | Получает [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот pivot cache. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот pivot cache. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Устанавливает количество неиспользуемых элементов, допускаемых до их удаления. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Освободить все ресурсы.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Получает количество неиспользуемых элементов, допускаемых до их удаления. Это значение ДОЛЖНО быть больше -2 и меньше 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Получает все сводные таблицы, использующие этот pivot cache.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Получает [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

См. [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот pivot cache.

**Remarks**

Если обе таблицы table1 и table2 используют этот кэш, обе таблицы будут вычислены. Лучше просто вызвать [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--), чтобы обновить все сводные таблицы и диаграммы в файле.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот pivot cache.

**Remarks**

Лучше просто вызвать [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--), чтобы обновить все сводные таблицы и диаграммы в файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Параметры обновления источника данных сводной таблицы. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Устанавливает количество неиспользуемых элементов, допускаемых до их удаления. Это значение ДОЛЖНО быть больше -2 и меньше 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

