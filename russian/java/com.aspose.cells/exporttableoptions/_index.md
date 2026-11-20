---
title: "ExportTableOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все параметры экспорта таблицы."
type: docs
url: /ru/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

Представляет все параметры экспорта таблицы.

**Remarks**

Если существуют особые требования к экспорту, например игнорирование ошибочных значений, пользователь может расширить этот класс, чтобы переопределить соответствующие API и достичь цели.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | Это значение указывает, разрешены ли DBNull в этой таблице. |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False, Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | Экспортирует строковое значение html ячеек в DataTable. |
| [getExportAsString()](#getExportAsString--) | Экспортирует строковое значение ячеек в DataTable. |
| [getExportColumnName()](#getExportColumnName--) | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. |
| [getFormatStrategy()](#getFormatStrategy--) | Получает стратегию форматирования при экспорте значения как строкового. |
| [getIndexes()](#getIndexes--) | Индексы столбцов/строк, которые следует экспортировать. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Экспортирует только видимые ячейки. |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | Экспортирует только видимые столбцы. |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | Экспортирует только видимые строки. |
| [getRenameStrategy()](#getRenameStrategy--) | Стратегия для дублирующих имён столбцов. |
| [getSkipErrorValue()](#getSkipErrorValue--) | Указывает, следует ли пропускать недопустимое значение для столбца. |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | True, если строка в файле Workbook представляет строку в DataTable. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | Предобработать значение текущей ячейки для экспорта. |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | Это значение указывает, разрешены ли DBNull в этой таблице. |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False, Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | Экспортирует строковое значение html ячеек в DataTable. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Экспортирует строковое значение ячеек в DataTable. |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | Указывает, экспортируются ли данные первой строки в имена столбцов DataTable. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Устанавливает стратегию форматирования при экспорте значения как строкового. |
| [setIndexes(int[] value)](#setIndexes-int---) | Индексы столбцов/строк, которые следует экспортировать. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Экспортирует только видимые ячейки. |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | Экспортирует только видимые столбцы. |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | Экспортирует только видимые строки. |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | Стратегия для дублирующих имён столбцов. |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | Указывает, следует ли пропускать недопустимое значение для столбца. |
| [setVertical(boolean value)](#setVertical-boolean-) | True, если строка в файле Workbook представляет строку в DataTable. |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


Это значение указывает, разрешены ли DBNull в этой таблице.

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False, Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. True, Aspose.Cells проверит, смешаны ли типы значений в столбце перед установкой типа DataColumn, и если типы смешаны, тип DataColumn будет строковым.

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


Экспортирует строковое значение html ячеек в DataTable.

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Экспортирует строковое значение ячеек в DataTable.

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


Указывает, экспортируются ли данные первой строки в имя столбца DataTable. Значение по умолчанию — false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Получает стратегию форматирования при экспорте значения как строкового.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Значение по умолчанию — [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


Индексы столбцов/строк, которые следует экспортировать.

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Экспортирует только видимые ячейки.

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


Экспортирует только видимые столбцы.

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


Экспортирует только видимые строки.

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


Стратегия для дублирующих имён столбцов.

См. [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


Указывает, следует ли пропускать недопустимое значение для столбца. Например, если тип столбца — decimal, значение превышает decimal.MaxValue и это свойство равно true, исключение выброшено не будет. Значение по умолчанию — false.

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


True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable.

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


Предобработать значение текущей ячейки для экспорта.

**Remarks**

Индекс строки и столбца — абсолютный индекс ячейки в листе, а не индекс в экспортируемой таблице. Пользователь может проверить значение текущей ячейки в переопределённой реализации этого метода; если текущую ячейку нужно заменить другим типом и значением, реализация должна установить ожидаемый тип и значение в объект CellValue и вернуть true. По умолчанию этот метод ничего не делает и возвращает false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellRow | int | индекс строки текущей ячейки |
| cellColumn | int | индекс столбца ячейки |
| value | [CellValue](../../com.aspose.cells/cellvalue) | значение и тип текущей ячейки |

**Returns:**
boolean — заменена ли текущая ячейка другим типом и/или значением.
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


Это значение указывает, разрешены ли DBNull в этой таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


False, Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности. True, Aspose.Cells проверит, смешаны ли типы значений в столбце перед установкой типа DataColumn, и если типы смешаны, тип DataColumn будет строковым.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


Экспортирует строковое значение html ячеек в DataTable.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Экспортирует строковое значение ячеек в DataTable.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


Указывает, экспортируются ли данные первой строки в имя столбца DataTable. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Устанавливает стратегию форматирования при экспорте значения как строкового.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Значение по умолчанию — [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


Индексы столбцов/строк, которые следует экспортировать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Экспортирует только видимые ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


Экспортирует только видимые столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


Экспортирует только видимые строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


Стратегия для дублирующих имён столбцов.

См. [RenameStrategy](../../com.aspose.cells/renamestrategy).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


Указывает, следует ли пропускать недопустимое значение для столбца. Например, если тип столбца — decimal, значение превышает decimal.MaxValue и это свойство равно true, исключение выброшено не будет. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


True, если строка в файле Workbook представляет строку в DataTable. False, если столбец в файле Workbook представляет строку в DataTable.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

