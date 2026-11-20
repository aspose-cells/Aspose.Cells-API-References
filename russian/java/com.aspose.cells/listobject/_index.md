---
title: "ListObject"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет таблицу в листе."
type: docs
url: /ru/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Представляет таблицу в листе.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Применить стиль таблицы к диапазону. |
| [convertToRange()](#convertToRange--) | Преобразовать таблицу в диапазон. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Преобразовать таблицу в диапазон. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Отфильтровать таблицу. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Получает альтернативное описание. |
| [getAlternativeText()](#getAlternativeText--) | Получает альтернативный текст. |
| [getAutoFilter()](#getAutoFilter--) | Получает автофильтр этой таблицы. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Получает комментарий к таблице. |
| [getDataRange()](#getDataRange--) | Получает диапазон данных таблицы. |
| [getDataSourceType()](#getDataSourceType--) | Получает тип источника данных таблицы. |
| [getDisplayName()](#getDisplayName--) | Получает отображаемое имя таблицы. |
| [getEndColumn()](#getEndColumn--) | Получает конечный столбец диапазона. |
| [getEndRow()](#getEndRow--) | Получает конечную строку диапазона. |
| [getListColumns()](#getListColumns--) | Получает список [ListColumn](../../com.aspose.cells/listcolumn) этой таблицы. |
| [getQueryTable()](#getQueryTable--) | Получает связанную QueryTable. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Получает, отображает ли эта Table строку заголовка. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Указывает, применяется ли форматирование полос столбцов. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Указывает, применяется ли стиль к первому столбцу в таблице. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Указывает, применяется ли стиль к последнему столбцу в таблице. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Указывает, применяется ли форматирование полос строк. |
| [getShowTotals()](#getShowTotals--) | Получает, отображает ли эта Table строку итогов. |
| [getStartColumn()](#getStartColumn--) | Получает начальный столбец диапазона. |
| [getStartRow()](#getStartRow--) | Получает начальную строку диапазона. |
| [getTableStyleName()](#getTableStyleName--) | Получает имя стиля таблицы. |
| [getTableStyleType()](#getTableStyleType--) | Получает встроенный стиль таблицы. |
| [getXmlMap()](#getXmlMap--) | Получает [getXmlMap()](../../com.aspose.cells/listobject\\#getXmlMap--) используемый для этого списка. |
| [hasAutoFilter()](#hasAutoFilter--) | Указывает, применяется ли автофильтр к этой таблице. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Поместите формулу в ячейку таблицы. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Поместите формулу в ячейку таблицы. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Поместите значение в ячейку. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Поместите значение в ячейку. |
| [removeAutoFilter()](#removeAutoFilter--) | Удаляет автофильтр, примененный к этой таблице. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Изменяет размер диапазона объекта списка. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Устанавливает альтернативное описание. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Устанавливает альтернативный текст. |
| [setComment(String value)](#setComment-java.lang.String-) | Устанавливает комментарий таблицы. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Устанавливает отображаемое имя таблицы. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Указывает, применяется ли автофильтр к этой таблице. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Устанавливает, отображает ли эта Table строку заголовка. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Указывает, применяется ли форматирование полос столбцов. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Указывает, применяется ли стиль к первому столбцу в таблице. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Указывает, применяется ли стиль к последнему столбцу в таблице. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Указывает, применяется ли форматирование полос строк. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Устанавливает, отображает ли эта TAble строку итогов. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Устанавливает имя стиля таблицы. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Получает встроенный стиль таблицы. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Обновляет имена всех столбцов списка в ячейки таблицы. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Применить стиль таблицы к диапазону.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Преобразовать таблицу в диапазон.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Преобразовать таблицу в диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | Параметры при преобразовании таблицы в диапазон. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Отфильтровать таблицу.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, установите свойство ListObject.HasAutoFilter./// Это свойство будет удалено через 12 месяцев, начиная с октября 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Получает альтернативное описание.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Получает альтернативный текст.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Получает автофильтр этой таблицы.

**Remarks**

Работает только когда [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) равно false.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Получает комментарий к таблице.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Получает диапазон данных таблицы.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Получает тип источника данных таблицы.

Смотрите [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Получает отображаемое имя таблицы.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Получает конечный столбец диапазона.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Получает конечную строку диапазона.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Получает список [ListColumn](../../com.aspose.cells/listcolumn) этой таблицы.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Получает связанную QueryTable.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Получает, отображает ли эта Table строку заголовка.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Указывает, применяется ли форматирование полос столбцов.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Указывает, применяется ли стиль к первому столбцу в таблице.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Указывает, применяется ли стиль к последнему столбцу в таблице.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Указывает, применяется ли форматирование полос строк.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Получает, отображает ли эта Table строку итогов.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Получает начальный столбец диапазона.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Получает начальную строку диапазона.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Получает имя стиля таблицы.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Получает встроенный стиль таблицы.

Смотрите [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Получает [getXmlMap()](../../com.aspose.cells/listobject\\#getXmlMap--) используемый для этого списка.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Указывает, применяется ли автофильтр к этой таблице.

**Returns:**
boolean
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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Поместите формулу в ячейку таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в таблице. |
| columnOffset | int | Смещение столбца в таблице. |
| formula | java.lang.String | Формула ячейки. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Поместите формулу в ячейку таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в таблице. |
| columnOffset | int | Смещение столбца в таблице. |
| formula | java.lang.String | Формула ячейки. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Поместите значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в таблице. |
| columnOffset | int | Смещение столбца в таблице. |
| значение | java.lang.Object | Значение ячейки. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Поместите значение в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | Смещение строки в таблице. |
| columnOffset | int | Смещение столбца в таблице. |
| значение | java.lang.Object | Значение ячейки. |
| isTotalsRowLabel | boolean | Указывает, является ли это меткой для строки итогов, работает только для строки итогов. Если значение False и эта строка является строкой итогов, будет вставлена новая строка. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Удаляет автофильтр, примененный к этой таблице.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Изменяет размер диапазона объекта списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Индекс начальной строки нового диапазона. |
| startColumn | int | Индекс начального столбца нового диапазона. |
| endRow | int | Индекс конечной строки нового диапазона. |
| endColumn | int | Индекс конечного столбца нового диапазона. |
| hasHeaders | boolean | Наличие заголовков в этой таблице. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Устанавливает альтернативное описание.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Устанавливает альтернативный текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Устанавливает комментарий таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Устанавливает отображаемое имя таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Указывает, применяется ли автофильтр к этой таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Устанавливает, отображает ли эта Table строку заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Указывает, применяется ли форматирование полос столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Указывает, применяется ли стиль к первому столбцу в таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Указывает, применяется ли стиль к последнему столбцу в таблице.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Указывает, применяется ли форматирование полос строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Устанавливает, отображает ли эта TAble строку итогов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Устанавливает имя стиля таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Получает встроенный стиль таблицы.

Смотрите [TableStyleType](../../com.aspose.cells/tablestyletype).

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
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Обновляет имена всех столбцов списка в ячейки таблицы.

**Remarks**

Значения ячеек в строке заголовка таблицы должны совпадать с именем ListColumn; Cell.PutValue не изменяет автоматически имя ListColumn в целях повышения производительности.

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

