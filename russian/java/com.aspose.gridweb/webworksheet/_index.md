---
title: "WebWorksheet"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет веб‑рабочий лист."
type: docs
url: /ru/java/com.aspose.gridweb/webworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class WebWorksheet extends Control
```

Представляет веб‑рабочий лист.

**Remarks**

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Пожалуйста, используйте GridWorksheet вместо него. Этот класс будет удалён через 6 месяцев, начиная с августа 2014 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WebWorksheet(MainWeb mw, GridWorksheet gwk)](#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | конструктор WebWorksheet. |
| [WebWorksheet()](#WebWorksheet--) | конструктор WebWorksheet. |
## Методы

| Метод | Описание |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Автоматически подгоняет ширину столбца. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Автоматически подгоняет ширину столбца. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Отменяет и удаляет недавно добавленную привязанную строку. |
| [commitNewBindRow()](#commitNewBindRow--) | Подтверждает недавно добавленную привязанную строку и добавляет её в источник данных. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Копирует из другого объекта листа. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | После установки источника данных для листа вызовите этот метод, чтобы автоматически создать привязанные столбцы. |
| [createNewBindRow()](#createNewBindRow--) | Создаёт новую привязанную строку и привязывает её к источнику данных. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Создаёт промежуточный итог на листе. |
| [dataBind()](#dataBind--) | Привяжите лист к источнику данных. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Удаляет привязанную строку. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Замораживает области в указанной ячейке листа. |
| [getBindStartColumn()](#getBindStartColumn--) | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [getBindStartRow()](#getBindStartRow--) | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [getBindingSource()](#getBindingSource--) | Фактический объект источника данных, привязываемый во время выполнения. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Получает количество привязанных строк в режиме привязки данных. |
| [getDataMember()](#getDataMember--) | Получает DataMember из многокомпонентного источника данных. |
| [getDataSource()](#getDataSource--) | Получает источник данных. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | В режиме привязки данных указывает, создавать ли подписи заголовков привязанных столбцов в листе. |
| [getIndex()](#getIndex--) | Получает свой индекс среди листов. |
| [getName()](#getName--) | Получает имя листа. |
| [getUniqueID()](#getUniqueID--) | Получает UniqueID в элементе управления. |
| [getValidations()](#getValidations--) | Получает коллекцию настроек проверки данных в листе. |
| [getVisible()](#getVisible--) | Указывает, отображается ли имя этого листа во вкладках листов элемента управления. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Группирует строки. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Группирует строки. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Получает, защищён ли лист. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Делает все ячейки редактируемыми. Это расширенный атрибут |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Делает все ячейки только для чтения. Это расширенный атрибут; обратите внимание, что этот атрибут не сохраняется в реальной ячейке, если вы хотите сохранить защиту, используйте setProtect. |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Получает количество привязанных строк в режиме привязки данных. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Устанавливает DataMember из многокомпонентного DataSource. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Устанавливает DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Делает все ячейки только для чтения, вызывая метод SetAllCellsReadonly. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | В режиме привязки данных указывает, создавать ли подписи заголовков привязанных столбцов в листе. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя листа. |
| [setProtected(boolean value)](#setProtected-boolean-) | Устанавливает, защищён ли лист. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, отображается ли имя этого листа во вкладках листов элемента управления. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Размораживает области в листе. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Разгруппирует строки. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WebWorksheet(MainWeb mw, GridWorksheet gwk) {#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WebWorksheet(MainWeb mw, GridWorksheet gwk)
```


конструктор WebWorksheet.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### WebWorksheet() {#WebWorksheet--}
```
public WebWorksheet()
```


конструктор WebWorksheet.

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Автоматически подгоняет ширину столбца.

**Remarks**

AutoFitColumn является неточной функцией.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Автоматически подгоняет ширину столбца. Этот метод автоматически подгоняет столбец на основе содержимого в диапазоне ячеек внутри столбца от startRow до endRow. AutoFitColumn — неточная функция.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | индекс столбца, начиная с нуля |
| startRow | int | индекс начальной строки, начиная с нуля |
| endRow | int | индекс конечной строки, начиная с нуля |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Отменяет и удаляет недавно добавленную привязанную строку.

**Returns:**
int — индекс строки. Если новая привязанная строка не создана, возвращает -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Подтверждает недавно добавленную привязанную строку и добавляет её в источник данных.

**Returns:**
int — индекс новой строки. Если строка не создана, возвращает -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Копирует из другого объекта листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | Другой лист. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


После установки источника данных для листа вызовите этот метод, чтобы автоматически создать привязанные столбцы.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Создаёт новую привязанную строку и привязывает её к источнику данных.

**Returns:**
int — индекс новой строки. Если строка не создана, возвращает -1.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Создаёт промежуточный итог на листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnNameRowIndex | int | Индекс строки названия столбца. |
| dataRows | int | Количество строк данных. |
| groupByColumnIndex | int | Индекс столбца, который будет группироваться. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Тип функции subtotal. |
| subtotalColumnIndexList | int[] | Индексы столбцов, подлежащих подсчету итогов. |
| functionLabel | java.lang.String | Метка функции subtotal. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Стиль строки общего итога. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Стиль строки промежуточного итога. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Тип числа ячеек результата subtotal. |
| customString | java.lang.String | Пользовательская строка формата ячеек результата subtotal. Может быть null. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Привяжите лист к источнику данных.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Удаляет привязанную строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNum | int | Индекс строки. |

**Returns:**
int — индекс удалённой строки. Если привязанная строка не удалена, возвращает -1.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Замораживает области в указанной ячейке листа.

**Remarks**

Индекс строки и индекс столбца не могут одновременно быть нулевыми. Количество строк и количество столбцов также не могут одновременно быть нулевыми.

Первые два параметра задают замороженную позицию, а последние два параметра задают область, замороженную в левом верхнем окне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |
| freezedRows | int | Количество видимых строк в верхней панели, не более индекса строки. |
| freezedColumns | int | Количество видимых столбцов в левой панели, не более индекса столбца. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


Фактический объект привязывающего datasource во время выполнения. Это объект DataView, когда свойство DataSource является объектом DataSet, DataTable или DataView.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Получает количество привязанных строк в режиме привязки данных.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Получает DataMember из многокомпонентного DataSource. Обычно он представляет объект DataTable из DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Получает DataSource. Обычно это объект DataSet.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


В режиме привязки данных указывает, создавать ли подписи заголовков привязанных столбцов в листе.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает свой индекс среди листов.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя листа.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Получает UniqueID в элементе управления.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Получает коллекцию настроек проверки данных в листе.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Указывает, отображается ли имя этого листа во вкладках листов элемента управления.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Группирует строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс строки для группировки. |
| lastIndex | int | Последний индекс строки для группировки. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Группирует строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Первый индекс строки для группировки. |
| lastIndex | int | Последний индекс строки для группировки. |
| isHidden | boolean | Указывает, скрыты ли сгруппированные строки. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Получает, защищён ли лист. Когда лист защищён, все ячейки нельзя редактировать, кроме ячейки, у которой свойство IsLocked равно false.

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




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Делает все ячейки редактируемыми. Это расширенный атрибут

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Делает все ячейки только для чтения. Это расширенный атрибут; обратите внимание, что этот атрибут не сохраняется в реальной ячейке, если вы хотите сохранить защиту, используйте setProtect.

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


В режиме привязки данных BindStartRow и BindStartColumn указывают позицию сетки для привязки к источнику данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Получает количество привязанных строк в режиме привязки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Устанавливает DataMember из многокомпонентного DataSource. Обычно он представляет объект DataTable из DataSet.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Устанавливает DataSource. Обычно это объект DataSet.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сделайте все ячейки только для чтения, вызвав метод SetAllCellsReadonly. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет редактируемым.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка диапазона. |
| startColumn | int | Начальный столбец диапазона. |
| строки | int | Количество строк. |
| столбцы | int | Количество столбцов. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


В режиме привязки данных указывает, создавать ли подписи заголовков привязанных столбцов в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Устанавливает, защищён ли лист. Когда лист защищён, все ячейки нельзя редактировать, кроме ячейки, у которой свойство IsLocked равно false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. Затем вызовите этот метод, чтобы указать диапазон ячеек, который будет только для чтения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка диапазона. |
| startColumn | int | Начальный столбец диапазона. |
| строки | int | Количество строк. |
| столбцы | int | Количество столбцов. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, отображается ли имя этого листа во вкладках листов элемента управления.

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
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Размораживает области в листе.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Разгруппирует строки.

**Remarks**

Только удаляет внешнюю информацию о группе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первой строки, которую нужно разгруппировать. |
| lastIndex | int | Индекс последней строки, которую нужно разгруппировать. |

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

