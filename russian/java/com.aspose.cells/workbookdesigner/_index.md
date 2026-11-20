---
title: "WorkbookDesigner"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий дизайнерскую электронную таблицу."
type: docs
url: /ru/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Инкапсулирует объект, представляющий дизайнерскую электронную таблицу.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Инициализирует новый экземпляр класса [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Инициализирует новый экземпляр класса [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## Методы

| Метод | Описание |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Очищает все источники данных. |
| [containsVariables()](#containsVariables--) | Указывает, содержит ли первый лист пользовательские переменные. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Указывает, следует ли вычислять формулы. |
| [getCallBack()](#getCallBack--) | Получает интерфейс обратного вызова обработки smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Указывает, содержит ли верхний/нижний колонтитул смарт‑марки и должны ли они обрабатываться вместе. |
| [getLineByLine()](#getLineByLine--) | Указывает, обрабатывается ли смарт‑маркер построчно. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Указывает, повторяются ли формулы с строкой подытога. |
| [getSmartMarkers()](#getSmartMarkers--) | Возвращает коллекцию смарт‑маркировок в электронной таблице. |
| [getSortDataSource()](#getSortDataSource--) | Указывает, сортировать ли источник данных. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Если TRUE, будет вставлен Null, если значение равно ""; |
| [getUpdateReference()](#getUpdateReference--) | Указывает, будут ли ссылки в других листах обновлены. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Получает имя листа, содержащего переменные смарт‑марки. |
| [getWorkbook()](#getWorkbook--) | Получает объект [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Обрабатывает смарт‑марки и заполняет значения источника данных. |
| [process(boolean isPreserved)](#process-boolean-) | Обрабатывает смарт‑марки и заполняет значения источника данных. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Обрабатывает смарт‑марки и заполняет значения источника данных. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Обрабатывает смарт‑марки и заполняет значения источника данных. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Указывает, следует ли вычислять формулы. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Устанавливает интерфейс обратного вызова обработки смарт‑маркера. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Указывает, содержит ли первый лист пользовательские переменные. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Устанавливает источник данных объекта [ICellsDataTable](../../com.aspose.cells/icellsdatatable). |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Устанавливает привязку данных к переменной. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Установите источник данных. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Установите источник данных. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Установите источник данных. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Указывает, содержит ли верхний/нижний колонтитул смарт‑марки и должны ли они обрабатываться вместе. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Установите строковое значение JSON в качестве источника данных смарт‑маркеров. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Указывает, обрабатывается ли смарт‑маркер построчно. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Указывает, повторяются ли формулы с строкой подытога. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Указывает, сортировать ли источник данных. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Если TRUE, будет вставлен Null, если значение равно ""; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Указывает, будут ли ссылки в других листах обновлены. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Устанавливает имя листа, содержащего переменные смарт‑марки. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Устанавливает объект [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Инициализирует новый экземпляр класса [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Инициализирует новый экземпляр класса [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Файл шаблона рабочей книги. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Очищает все источники данных.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Указывает, содержит ли первый лист пользовательские переменные.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство WorkbookDesigner.VariablesWorksheetName. Это свойство будет удалено через 3 месяца, начиная с сентября 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Указывает, следует ли вычислять формулы.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Получает интерфейс обратного вызова обработки smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Указывает, содержит ли верхний/нижний колонтитул смарт‑марки и должны ли они обрабатываться вместе.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Указывает, обрабатывается ли смарт‑маркер построчно.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте range smart markers. Это свойство будет удалено через 12 месяцев, начиная с июля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Указывает, повторяются ли формулы с строкой подытога.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Возвращает коллекцию смарт‑маркировок в электронной таблице.

**Remarks**

Массив строк создаётся при каждом вызове. Массив сортируется, а дублированные значения удаляются.

**Returns:**
java.lang.String[] — коллекция смарт‑маркировок
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Указывает, сортировать ли источник данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Оно будет удалено через 12 месяцев, начиная с октября 2026 года. Aspose приносит извинения за любые причинённые неудобства. JSON‑источник данных будет отсортирован, если смарт‑маркер содержит параметры сортировки по возрастанию и убыванию.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Если TRUE, будет вставлен Null, если значение равно "";

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Указывает, будут ли ссылки в других листах обновлены.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Получает имя листа, содержащего переменные смарт‑марки.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Обрабатывает смарт‑марки и заполняет значения источника данных.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Обрабатывает смарт‑марки и заполняет значения источника данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isPreserved | boolean | True, если нераспознанный смарт‑маркер сохраняется. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Обрабатывает смарт‑марки и заполняет значения источника данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Range smart markers. Это свойство будет удалено через 12 месяцев, начиная с июля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Диапазон для обработки |
| isPreserved | boolean | True, если нераспознанный смарт‑маркер сохраняется. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Обрабатывает смарт‑марки и заполняет значения источника данных.

**Remarks**

Этот метод работает на уровне листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа. |
| isPreserved | boolean | True, если нераспознанный смарт‑маркер сохраняется. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Указывает, следует ли вычислять формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Устанавливает интерфейс обратного вызова обработки смарт‑маркера.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Указывает, содержит ли первый лист пользовательские переменные.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство WorkbookDesigner.VariablesWorksheetName. Это свойство будет удалено через 3 месяца, начиная с сентября 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Устанавливает источник данных объекта [ICellsDataTable](../../com.aspose.cells/icellsdatatable).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSource | java.lang.String | Имя источника данных. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | таблица данных. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Устанавливает привязку данных к переменной.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| variable | java.lang.String | Имя переменной, созданное с помощью смарт‑маркира. |
| данные | java.lang.Object | Исходные данные. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Установите источник данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSource | java.lang.String | Имя источника данных. |
| rs | java.sql.ResultSet | Набор результатов. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Установите источник данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSource | java.lang.String | Имя источника данных. |
| rs | java.sql.ResultSet | Набор результатов. |
| rowCount | int | Количество данных в данном наборе результатов. Оно должно быть точным количеством строк или -1; если набор результатов только для чтения вперёд, пользователь должен указать точное количество строк здесь, иначе смарт‑маркер может быть обработан некорректно, когда у смарт‑маркира не установлен параметр \"noadd\". |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Установите источник данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rs | java.sql.ResultSet | Набор результатов. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Указывает, содержит ли верхний/нижний колонтитул смарт‑марки и должны ли они обрабатываться вместе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Установите строковое значение JSON в качестве источника данных смарт‑маркеров.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя таблицы. Если значение JSON представляет объект, оно может быть null. |
| json | java.lang.String | Значение строки Json. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Указывает, обрабатывается ли смарт‑маркер построчно.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте range smart markers. Это свойство будет удалено через 12 месяцев, начиная с июля 2025 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Указывает, повторяются ли формулы с строкой подытога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Указывает, сортировать ли источник данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Оно будет удалено через 12 месяцев, начиная с октября 2026 года. Aspose приносит извинения за любые причинённые неудобства. JSON‑источник данных будет отсортирован, если смарт‑маркер содержит параметры сортировки по возрастанию и убыванию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Если TRUE, будет вставлен Null, если значение равно "";

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Указывает, будут ли ссылки в других листах обновлены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Устанавливает имя листа, содержащего переменные смарт‑марки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Устанавливает объект [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

