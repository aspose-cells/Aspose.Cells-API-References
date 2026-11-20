---
title: "PivotTableCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет коллекцию всех объектов PivotTable на указанном листе."
type: docs
url: /ru/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Представляет коллекцию всех объектов PivotTable на указанном листе.

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
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Добавляет новую сводную таблицу на основе другой сводной таблицы. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Добавляет новую сводную таблицу на основе другой сводной таблицы. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Добавляет новую сводную таблицу в указанную строку и столбец листа. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Добавляет новую сводную таблицу. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных. |
| [clear()](#clear--) | Очищает все сводные таблицы. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает отчет сводной таблицы по индексу. |
| [get(int row, int column)](#get-int-int-) | Получает [PivotTable](../../com.aspose.cells/pivottable), расположенный в ячейке. |
| [get(String name)](#get-java.lang.String-) | Получает отчет сводной таблицы по имени сводной таблицы. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Удаляет указанную сводную таблицу и удаляет данные сводной таблицы. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Удаляет указанную сводную таблицу. |
| [removeAt(int index)](#removeAt-int-) | Удаляет сводную таблицу по указанному индексу и удаляет данные сводной таблицы. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Удаляет сводную таблицу по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Добавляет новую сводную таблицу на основе другой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Исходная сводная таблица. |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленной сводной таблицы.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Добавляет новую сводную таблицу на основе другой сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Исходная сводная таблица. |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленной сводной таблицы.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | int | Нулевой индекс строки левого верхнего угла назначения сводной таблицы. |
| столбец | int | Нулевой индекс столбца левого верхнего угла назначения сводной таблицы. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Добавляет новую сводную таблицу в указанную строку и столбец листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | int | Нулевой индекс строки левого верхнего угла назначения сводной таблицы. |
| столбец | int | Нулевой индекс столбца левого верхнего угла назначения сводной таблицы. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Параметры создания сводной таблицы. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за возможные неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс в этом списке сводных таблиц.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за возможные неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |
| useSameSource | boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использует этот источник данных. Если свойство истинно, это сэкономит память. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после октября 2026 года. Приносим извинения за любые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |
| useSameSource | boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использует этот источник данных. Если свойство истинно, это сэкономит память. |
| isXlsClassic | boolean | Указывает, следует ли добавить классическую сводную таблицу Excel 97-2003. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| cellName | java.lang.String | Имя ячейки в левом верхнем углу назначения сводной таблицы. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Добавляет новую современную сводную таблицу (с Excel 2007) в указанную строку и столбец листа с параметрами по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| cellName | java.lang.String | Имя ячейки в левом верхнем углу назначения сводной таблицы. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Параметры создания сводной таблицы. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за возможные неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Данные для нового кэша сводной таблицы. |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс в этом списке сводных таблиц.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после сентября 2026 года. Приносим извинения за возможные неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Данные для нового кэша сводной таблицы. |
| destCellName | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |
| useSameSource | boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использует этот источник данных. Если свойство истинно, это сэкономит память. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Добавляет новую сводную таблицу.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод устарел. Он эквивалентен вызову PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) с `NewPivotTableOptions.IsXlsClassic = true`. Пожалуйста, используйте перегрузку PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) вместо этого. Этот метод будет удалён через 12 месяцев после октября 2026 года. Приносим извинения за любые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8 |
| ячейка | java.lang.String | Ячейка в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |
| useSameSource | boolean | Указывает, использовать ли тот же источник данных, когда другая существующая сводная таблица уже использовала этот источник данных. Если свойство истинно, это сэкономит память, когда один и тот же источник данных собран в один кэш сводных таблиц. |
| isXlsClassic | boolean | Указывает, следует ли добавить классическую сводную таблицу Excel 97-2003. |

**Returns:**
int — Индекс только что добавленного кэша.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String[] | Несколько диапазонов консолидации, например \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Создавать ли автоматически единственное поле страницы. Если истинно, параметр pageFields будет игнорироваться. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Элементы поля страницы сводной таблицы. |
| строка | int | Индекс строки ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| столбец | int | Индекс столбца ячейки в левом верхнем углу диапазона назначения отчета сводной таблицы. |
| tableName | java.lang.String | Имя нового отчета сводной таблицы. |

**Returns:**
int — Индекс только что добавленной сводной таблицы.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceData | java.lang.String[] | Несколько диапазонов консолидации, например \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Создавать ли автоматически единственное поле страницы. Если истинно, параметр pageFields будет игнорироваться. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Элементы поля страницы сводной таблицы. |
| destCellName | java.lang.String | destCellName Имя нового отчёта сводной таблицы. |
| tableName | java.lang.String | имя нового отчёта сводной таблицы. |

**Returns:**
int — Индекс только что добавленной сводной таблицы.
### clear() {#clear--}
```
public void clear()
```


Очищает все сводные таблицы.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


Получает отчет сводной таблицы по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Получает [PivotTable](../../com.aspose.cells/pivottable), расположенный в ячейке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int |  |
| столбец | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Получает отчет сводной таблицы по имени сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Удаляет указанную сводную таблицу и удаляет данные сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Удаляет указанную сводную таблицу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Объект PivotTable |
| keepData | boolean | Нужно ли сохранять данные сводной таблицы |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет сводную таблицу по указанному индексу и удаляет данные сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс позиции в коллекции сводных таблиц |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Удаляет сводную таблицу по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс позиции в коллекции сводных таблиц |
| keepData | boolean | Нужно ли сохранять данные сводной таблицы |

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

