---
title: "FormatConditionCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет условное форматирование."
type: docs
url: /ru/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Представляет условное форматирование. Объект FormatConditions может содержать до трёх условных форматов.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. Объект FormatConditions может содержать до трёх условных форматов. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Добавляет диапазон ячеек с условным форматированием. |
| [addCondition(int type)](#addCondition-int-) | Добавить условие форматирования. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Добавляет условие форматирования. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает условие форматирования по индексу. |
| [getCellArea(int index)](#getCellArea-int-) | Получает диапазон ячеек с условным форматированием по индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество условий. |
| [getRangeCount()](#getRangeCount--) | Получает количество диапазонов с условным форматированием. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Удаляет диапазон ячеек с условным форматированием по индексу. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Удалить условное форматирование в диапазоне. |
| [removeCondition(int index)](#removeCondition-int-) | Удаляет условие форматирования по индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. FormatConditions могут содержать до трех условных форматов. Ссылки на другие листы не допускаются в формулах условного форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Диапазон ячеек с условным форматированием. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Тип условного форматирования. Может быть одним из членов FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Оператор сравнения. Может быть одним из членов OperatorType. |
| formula1 | java.lang.String | Значение или выражение, связанное с условным форматированием. |
| formula2 | java.lang.String | Значение или выражение, связанное с условным форматированием |

**Returns:**
int[] - [0]:Индекс объекта условия форматирования;[1] Индекс затронутого диапазона ячеек.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Добавляет диапазон ячеек с условным форматированием.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Диапазон ячеек с условным форматированием. |

**Returns:**
int - Индекс диапазона ячеек с условным форматированием.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Добавить условие форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Тип условия форматирования. |

**Returns:**
int - Индекс объекта условия форматирования;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Добавляет условие форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Тип условия форматирования. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Тип оператора |
| formula1 | java.lang.String | Значение или выражение, связанное с условным форматированием. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: \"=\\\\\"=...\\\\\"\". |
| formula2 | java.lang.String | Значение или выражение, связанное с условным форматированием. Формат ввода такой же, как у formula1 |

**Returns:**
int - Индекс объекта условия форматирования;
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
public FormatCondition get(int index)
```


Получает условие форматирования по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс условия форматирования, которое нужно вернуть. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Получает диапазон ячеек с условным форматированием по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | индекс диапазона ячеек с условным форматированием. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
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


Получает количество условий.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Получает количество диапазонов с условным форматированием.

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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Удаляет диапазон ячеек с условным форматированием по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс диапазона ячеек с условным форматированием, который нужно удалить. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Удалить условное форматирование в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка (startRow) диапазона. |
| startColumn | int | Начальный столбец (startColumn) диапазона. |
| totalRows | int | Количество строк в диапазоне. |
| totalColumns | int | Количество столбцов в диапазоне. |

**Returns:**
boolean - Возвращает TRUE, эта коллекция FormatCondtionCollection должна быть удалена.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Удаляет условие форматирования по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс условия форматирования, которое нужно удалить. |

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

