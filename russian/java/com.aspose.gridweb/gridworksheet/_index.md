---
title: "GridWorksheet"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий отдельный лист."
type: docs
url: /ru/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Инкапсулирует объект, представляющий отдельный лист.
## Методы

| Метод | Описание |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Устанавливает диапазон, к которому применяется указанный AutoFilter. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Добавить пользовательский фильтр для указанной строки. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Автоматически подгоняет ширину столбца. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Автоматически подгоняет ширину столбца. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Автоматически подгоняет высоту строки. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Автоматически подгоняет высоту строки. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Автоматически подгоняет высоту строки в прямоугольном диапазоне. |
| [autoFitRows()](#autoFitRows--) | Автоматически подгоняет высоту всех строк в этом листе. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Автоматически подгоняет высоту всех строк в этом листе. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Автоматически подгоняет высоту строки в диапазоне. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Вычисляет формулу. |
| [clearComments()](#clearComments--) | Очищает все комментарии в дизайнерской таблице. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Копирует содержимое и форматы из другого листа. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Создаёт промежуточный итог на листе. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Создаёт промежуточный итог на листе. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Устанавливает фильтр для столбца. Обратите внимание, что необходимо вызвать AddAutoFilter перед вызовом filterString. Строка критериев фильтра. Обратите внимание, что мы используем запятую -> "," в качестве разделителя, поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString(10,"123,456") означает, что столбец 10 должен содержать 123 или 456, filterString(10,"123") означает, что столбец 10 должен содержать 123. Индекс столбца может быть разделён запятыми, например 123,456,789 или abc. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Замораживает области в указанной ячейке листа. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Замораживает области в указанной ячейке листа. |
| [getActiveCell()](#getActiveCell--) | Получает активную ячейку в листе. |
| [getBackgroundImage()](#getBackgroundImage--) | Получает фоновое изображение листа. |
| [getCells()](#getCells--) | Получает коллекцию [GridCell](../../com.aspose.gridweb/gridcell). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Представляет кодовое имя листа. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Получает подпись столбца. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Получает текст всплывающей подсказки заголовка столбца. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Получает, является ли столбец только для чтения. |
| [getComments()](#getComments--) | Получает коллекцию [GridComment](../../com.aspose.gridweb/gridcomment). |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Указывает, отображается ли указанный лист справа налево вместо слева направо. |
| [getDisplayZeros()](#getDisplayZeros--) | True, если отображаются нулевые значения. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Представляет индекс первой видимой колонки. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Представляет индекс первой видимой строки. |
| [getFreezedPanes()](#getFreezedPanes--) | Получает замороженные области. |
| [getGridActiveCell()](#getGridActiveCell--) | Получает активную ячейку в листе. |
| [getHyperlinks()](#getHyperlinks--) | Получает коллекцию [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection). |
| [getIndex()](#getIndex--) | Получает индекс листа в коллекции листов. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Получает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, он не сохраняется в реальном файле Excel. |
| [getName()](#getName--) | Получает имя листа. |
| [getOutlineShown()](#getOutlineShown--) | Указывает, показывать ли контур. |
| [getPictures()](#getPictures--) | Получает коллекцию [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--). |
| [getPivotTables()](#getPivotTables--) | Получает сводные таблицы на листе. |
| [getRowCaption(int row)](#getRowCaption-int-) | Получает подпись строки. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Получает текст всплывающей подсказки заголовка строки. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Получает, является ли строка только для чтения. |
| [getSelected()](#getSelected--) | Указывает, будет ли этот лист выбран при открытии книги. |
| [getShapes()](#getShapes--) | Получает коллекцию [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--). |
| [getStandardHeight()](#getStandardHeight--) | Получает высоту строки по умолчанию в этом листе, в пунктах. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Получает высоту строки по умолчанию в этом листе, в пикселях. |
| [getTabColor()](#getTabColor--) | Представляет цвет вкладки листа. |
| [getUniqueID()](#getUniqueID--) | Получает UniqueID в элементе управления. |
| [getValidations()](#getValidations--) | Получает коллекцию настроек проверки данных в листе. |
| [getVisible()](#getVisible--) | Указывает, отображается ли имя этого листа во вкладках листов элемента управления. |
| [getWorkbook()](#getWorkbook--) | Получает объект [GridWorkbook](../../com.aspose.gridweb/gridworkbook) коллекции листов. |
| [getZoom()](#getZoom--) | Представляет коэффициент масштабирования в процентах. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Группирует строки. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Получает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [isProtected()](#isProtected--) | Указывает, защищён ли лист. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Указывает, будет ли строка итога размещена ниже строк деталей в контуре. |
| [moveTo(int index)](#moveTo-int-) | Перемещает лист в другое место в таблице. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Обновить автофильтры, чтобы скрыть или показать строки. |
| [removeAutoFilter()](#removeAutoFilter--) | Удалить автофильтр листа. |
| [removeSubtotal()](#removeSubtotal--) | Удаляет подытог, созданный методом CreateSubtotal на листе. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | Целочисленное смещение поля, к которому вы хотите применить, основанное на первом столбце фильтра (слева в списке; самый левый столбец — поле 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Устанавливает активную ячейку в листе. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Делает все ячейки редактируемыми. Это расширенный атрибут |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Делает все ячейки только для чтения. Это расширенный атрибут; обратите внимание, что этот атрибут не сохраняется в реальной ячейке, если вы хотите сохранить защиту, используйте setProtect. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Устанавливает фоновое изображение листа. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Устанавливает подпись для столбца. Обратите внимание, что это расширенный атрибут и не сохраняется в файле Excel. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Устанавливает текст всплывающей подсказки заголовка столбца. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Устанавливает столбец только для чтения, чтобы пользователь не мог удалить его на клиентской стороне. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Указывает, отображается ли указанный лист справа налево вместо слева направо. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | True, если отображаются нулевые значения. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Делает диапазон ячеек редактируемым. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Делает все ячейки только для чтения, вызывая метод SetAllCellsReadonly. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Представляет индекс первой видимой колонки. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Представляет индекс первой видимой строки. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Устанавливает активную ячейку в листе. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Устанавливает значение, указывающее, видимы ли линии сетки. По умолчанию true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Устанавливает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, он не сохраняется в реальном файле Excel. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя листа. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Указывает, показывать ли контур. |
| [setProtect()](#setProtect--) | Защищает лист. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Делает диапазон ячеек только для чтения. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Сначала сделайте все ячейки редактируемыми, вызвав метод SetAllCellsEditable. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Устанавливает подпись для строки. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Устанавливает текст всплывающей подсказки заголовка строки. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Устанавливает строку только для чтения, чтобы пользователь не мог удалить её на клиентской стороне. |
| [setSelected(boolean value)](#setSelected-boolean-) | Указывает, будет ли этот лист выбран при открытии книги. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Устанавливает высоту строки по умолчанию в этом листе, в единицах точек. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Устанавливает высоту строки по умолчанию в этом листе, в единицах пикселей. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Указывает, будет ли строка итога размещена ниже строк деталей в контуре. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Представляет цвет вкладки листа. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, отображается ли имя этого листа во вкладках листов элемента управления. |
| [setZoom(int value)](#setZoom-int-) | Представляет коэффициент масштабирования в процентах. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Размораживает области в листе. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Разгруппирует строки. |
| [unProtect()](#unProtect--) | Снимает защиту с листа. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Устанавливает диапазон, к которому применяется указанный AutoFilter.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Добавить пользовательский фильтр для указанной строки.

**Remarks**

Строка критериев фильтра. Обратите внимание, что мы используем запятую и точку с запятой как разделители, поэтому значение ячейки не должно содержать эти разделители. Ниже приведены примеры строк критериев //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int |  |
| критерий | java.lang.String |  |

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

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Автоматически подгоняет ширину столбца.

**Remarks**

Этот метод автоматически подгоняет высоту строки на основе содержимого в диапазоне ячеек внутри строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Индекс столбца. |
| firstRow | int | Индекс первой строки. |
| lastRow | int | Индекс последней строки. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Автоматически подгоняет высоту строки.

**Remarks**

AutoFitRow — неточная функция.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Автоматически подгоняет высоту строки.

**Remarks**

Этот метод автоматически подгоняет высоту строки на основе содержимого в диапазоне ячеек внутри строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| firstColumn | int | Индекс первого столбца. |
| lastColumn | int | Последний индекс столбца. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Автоматически подгоняет высоту строки в прямоугольном диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |
| startColumn | int | Индекс начального столбца. |
| endColumn | int | Индекс конечного столбца. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Автоматически подгоняет высоту всех строк в этом листе.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Автоматически подгоняет высоту всех строк в этом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| onlyAuto | boolean | True, только автоматически подгоняет высоту строки, когда высота строки не настроена вручную. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Автоматически подгоняет высоту строки в диапазоне.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки. |
| endRow | int | Индекс конечной строки. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Вычисляет формулу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


Очищает все комментарии в дизайнерской таблице.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Копирует содержимое и форматы из другого листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Исходный лист. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Устанавливает фильтр для столбца. Обратите внимание, что необходимо вызвать AddAutoFilter перед вызовом filterString. Строка критериев фильтра. Обратите внимание, что мы используем запятую -> "," в качестве разделителя, поэтому значение ячейки, которое вы хотите отфильтровать, не должно содержать запятую. filterString(10,"123,456") означает, что столбец 10 должен содержать 123 или 456, filterString(10,"123") означает, что столбец 10 должен содержать 123. Индекс столбца может быть разделён запятыми, например 123,456,789 или abc.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int |  |
| критерий | java.lang.String |  |

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

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Замораживает области в указанной ячейке листа.

**Remarks**

Индекс строки и индекс столбца не могут одновременно быть нулевыми. Количество строк и количество столбцов также не могут одновременно быть нулевыми.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| freezedRows | int | Количество видимых строк в верхней панели, не более индекса строки. |
| freezedColumns | int | Количество видимых столбцов в левой панели, не более индекса столбца. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Получает активную ячейку в листе.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Получает фоновое изображение листа.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Получает коллекцию [GridCell](../../com.aspose.gridweb/gridcell).

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Представляет кодовое имя листа.

**Remarks**

Нельзя изменить имя кода, пока файл шаблона содержит VBA/макрос.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Получает подпись столбца. Если подпись не задана, возвращает пустую строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String - Подпись столбца. Если подпись не задана, возвращает пустую строку.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Получает текст всплывающей подсказки заголовка столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| colIndex | int | Индекс столбца. |

**Returns:**
java.lang.String - Текст всплывающей подсказки.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Получает, является ли столбец только для чтения. Это расширенный метод GridWeb, который не сохраняется и не влияет на реальный файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | индекс столбца. |

**Returns:**
boolean - Если только для чтения, возвращает true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Получает коллекцию [GridComment](../../com.aspose.gridweb/gridcomment).

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию — false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


True, если отображаются нулевые значения.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Представляет индекс первой видимой колонки.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Представляет индекс первой видимой строки.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Получает замороженные области.

**Returns:**
int[] - Возврат null означает, что лист не заморожен 0: индекс строки;1: столбец;2: замороженные строки;3: замороженные строки
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Получает активную ячейку в листе.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Получает коллекцию [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection).

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс листа в коллекции листов.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Получает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, он не сохраняется в реальном файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Получает имя листа.

**Remarks**

Максимальная длина имени листа — 31 символ. И вы не можете присвоить одинаковое имя (без учёта регистра) двум листам. Например, вы не можете установить "SheetName1" для первого листа и "SHEETNAME1" для второго листа.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Указывает, показывать ли контур.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Получает коллекцию [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--).

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Получает сводные таблицы на листе.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Получает подпись строки. Если подпись не задана, возвращает пустую строку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |

**Returns:**
java.lang.String - Подпись строки. Если подпись не задана, возвращает пустую строку.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Получает текст всплывающей подсказки заголовка строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |

**Returns:**
java.lang.String - Текст всплывающей подсказки.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Получает, является ли строка только для чтения. Это расширенный метод GridWeb, он не будет сохраняться и влиять на реальный файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | индекс строки. |

**Returns:**
boolean - Если только для чтения, возвращает true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Указывает, будет ли этот лист выбран при открытии книги.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Получает коллекцию [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--).

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Получает высоту строки по умолчанию в этом листе, в пунктах.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Получает высоту строки по умолчанию в этом листе, в пикселях.

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Представляет цвет вкладки листа.

**Remarks**

Эта функция поддерживается только в ExcelXP (Excel2002) и более новых версиях. Если сохранить файл в формате Excel97 или Excel2000, она будет опущена.

**Returns:**
[Color](../../com.aspose.gridweb/color)
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
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Получает объект [GridWorkbook](../../com.aspose.gridweb/gridworkbook) коллекции листов.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Представляет коэффициент масштабирования в процентах. Должен находиться в диапазоне от 10 до 400.

**Returns:**
int
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
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Получает значение, указывающее, видимы ли линии сетки. По умолчанию true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Указывает, защищён ли лист.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Указывает, будет ли строка итога размещена ниже строк деталей в контуре.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Перемещает лист в другое место в таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс листа назначения. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Обновить автофильтры, чтобы скрыть или показать строки.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Удалить автофильтр листа.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Удаляет подытог, созданный методом CreateSubtotal на листе.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


Целочисленное смещение поля, к которому вы хотите применить, основанное на первом столбце фильтра (слева в списке; самый левый столбец — поле 0).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Устанавливает активную ячейку в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Устанавливает фоновое изображение листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Устанавливает подпись для столбца. Обратите внимание, что это расширенный атрибут и не сохраняется в файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца. |
| заголовок | java.lang.String | Заголовок столбца. Передайте null или пустую строку, если хотите отменить заголовок. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Устанавливает текст всплывающей подсказки заголовка столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| colIndex | int | Индекс столбца. |
| подсказка | java.lang.String | Текст подсказки. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Устанавливает столбец только для чтения, чтобы пользователь не мог удалить его на клиентской стороне. Это расширенный метод GridWeb, он не будет сохраняться и влиять на реальный файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | индекс столбца. |
| isReadonly | boolean | true или false. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


True, если отображаются нулевые значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Представляет индекс первой видимой колонки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Представляет индекс первой видимой строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Устанавливает активную ячейку в листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Устанавливает значение, указывающее, видимы ли линии сетки. По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Устанавливает, является ли ячейка только для чтения. Это расширенный атрибут GridWeb, он не сохраняется в реальном файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int |  |
| col | int |  |
| значение | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя листа.

**Remarks**

Максимальная длина имени листа — 31 символ. И вы не можете присвоить одинаковое имя (без учёта регистра) двум листам. Например, вы не можете установить "SheetName1" для первого листа и "SHEETNAME1" для второго листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Указывает, показывать ли контур.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Защищает лист.

**Remarks**

Этот метод защищает лист без пароля. Он может защищать лист во всех версиях файлов Excel.

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

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Устанавливает подпись для строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| заголовок | java.lang.String | Заголовок строки. Передайте null или пустую строку, если хотите отменить заголовок. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Устанавливает текст всплывающей подсказки заголовка строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | Индекс строки. |
| подсказка | java.lang.String | Текст подсказки. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Устанавливает строку только для чтения, чтобы пользователь не мог удалить её на клиентской стороне. Это расширенный метод GridWeb, он не будет сохраняться и влиять на реальный файл Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int | индекс строки. |
| isReadonly | boolean | true или false. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Указывает, будет ли этот лист выбран при открытии книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Устанавливает высоту строки по умолчанию в этом листе, в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Устанавливает высоту строки по умолчанию в этом листе, в единицах пикселей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Указывает, будет ли строка итога размещена ниже строк деталей в контуре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Представляет цвет вкладки листа.

**Remarks**

Эта функция поддерживается только в ExcelXP (Excel2002) и более новых версиях. Если сохранить файл в формате Excel97 или Excel2000, она будет опущена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, отображается ли имя этого листа во вкладках листов элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Представляет коэффициент масштабирования в процентах. Должен находиться в диапазоне от 10 до 400.

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
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Размораживает области в листе.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Разгруппирует строки.

**Remarks**

Только удаляет внешнюю информацию о группе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | int | Индекс первой строки, которую нужно разгруппировать. |
| lastIndex | int | Индекс последней строки, которую нужно разгруппировать. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Снимает защиту с листа.

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

