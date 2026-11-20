---
title: "ImportTableOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры импорта данных в ячейки."
type: docs
url: /ru/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

Представляет параметры импорта данных в ячейки.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | Создаёт параметры импорта по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | Указывает, следует ли проверять объединённые ячейки. |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | Получает столбцы (нумерация с нуля), которые нужно импортировать из источника данных. null означает, что следует импортировать все столбцы. |
| [getConvertGridStyle()](#getConvertGridStyle--) | Указывает, применять ли стиль представления сетки к ячейкам. |
| [getConvertNumericData()](#getConvertNumericData--) | Получает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату. |
| [getDateFormat()](#getDateFormat--) | Получает строку формата даты для ячеек с импортированными значениями даты и времени. |
| [getDefaultValues()](#getDefaultValues--) | Значение по умолчанию для значения в таблице — null. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | Указывает, экспортировать ли подпись как имя поля. |
| [getInsertRows()](#getInsertRows--) | Указывает, следует ли добавлять новые строки при импорте записей данных. |
| [getNumberFormats()](#getNumberFormats--) | Получает числовые форматы. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | Указывает, следует ли сдвигать первую строку вниз при вставке строк. |
| [getStyles()](#getStyles--) | Получает стили для каждого столбца таблицы. |
| [getTotalColumns()](#getTotalColumns--) | Получает общее количество столбцов для импорта из источника данных. -1 означает все строки данного источника данных. |
| [getTotalRows()](#getTotalRows--) | Получает общее количество строк для импорта из источника данных. -1 означает все строки данного источника данных. |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | Указывает, следует ли импортировать имя поля. |
| [isFormulas()](#isFormulas--) | Указывает, являются ли данные формулами. |
| [isHtmlString()](#isHtmlString--) | Указывает, содержит ли значение HTML‑теги. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | Указывает, следует ли проверять объединённые ячейки. |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | Устанавливает столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы. |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | Указывает, применять ли стиль представления сетки к ячейкам. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Устанавливает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Устанавливает строку формата даты для ячеек с импортированными значениями даты и времени. |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | Значение по умолчанию для значения в таблице — null. |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | Указывает, экспортировать ли подпись как имя поля. |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | Указывает, следует ли импортировать имя поля. |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | Указывает, являются ли данные формулами. |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | Указывает, содержит ли значение HTML‑теги. |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | Указывает, следует ли добавлять новые строки при импорте записей данных. |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | Устанавливает числовые форматы |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | Указывает, следует ли сдвигать первую строку вниз при вставке строк. |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | Устанавливает стили для каждого столбца таблицы. |
| [setTotalColumns(int value)](#setTotalColumns-int-) | Устанавливает общее количество столбцов для импорта из источника данных. -1 означает все строки заданного источника данных. |
| [setTotalRows(int value)](#setTotalRows-int-) | Устанавливает общее количество строк для импорта из источника данных. -1 означает все строки заданного источника данных. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


Создаёт параметры импорта по умолчанию.

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


Указывает, следует ли проверять объединённые ячейки.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


Получает столбцы (нумерация с нуля), которые нужно импортировать из источника данных. null означает, что следует импортировать все столбцы.

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


Указывает, применять ли стиль представления сетки к ячейкам.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Получает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Получает строку формата даты для ячеек с импортированными значениями даты и времени.

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


Значение по умолчанию для значения в таблице — null.

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


Указывает, экспортировать ли подпись как имя поля.

**Remarks**

Работает только с DataTable.

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


Указывает, следует ли добавлять новые строки при импорте записей данных.

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


Получает числовые форматы.

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


Указывает, следует ли сдвигать первую строку вниз при вставке строк.

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


Получает стили для каждого столбца таблицы.

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


Получает общее количество столбцов для импорта из источника данных. -1 означает все строки данного источника данных.

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


Получает общее количество строк для импорта из источника данных. -1 означает все строки данного источника данных.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


Указывает, следует ли импортировать имя поля.

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


Указывает, являются ли данные формулами.

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


Указывает, содержит ли значение HTML‑теги.

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


Указывает, следует ли проверять объединённые ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


Устанавливает столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


Указывает, применять ли стиль представления сетки к ячейкам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Устанавливает значение, указывающее, следует ли преобразовать строковое значение в числовое или дату.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Устанавливает строку формата даты для ячеек с импортированными значениями даты и времени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


Значение по умолчанию для значения в таблице — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


Указывает, экспортировать ли подпись как имя поля.

**Remarks**

Работает только с DataTable.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


Указывает, следует ли импортировать имя поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


Указывает, являются ли данные формулами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


Указывает, содержит ли значение HTML‑теги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


Указывает, следует ли добавлять новые строки при импорте записей данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


Устанавливает числовые форматы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


Указывает, следует ли сдвигать первую строку вниз при вставке строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


Устанавливает стили для каждого столбца таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


Устанавливает общее количество столбцов для импорта из источника данных. -1 означает все строки заданного источника данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


Устанавливает общее количество строк для импорта из источника данных. -1 означает все строки заданного источника данных.

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

