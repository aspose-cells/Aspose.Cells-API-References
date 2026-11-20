---
title: "SqlScriptSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения sql."
type: docs
url: /ru/java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

Представляет параметры сохранения sql.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | Создаёт параметры для сохранения sql файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | Вставлять пустую строку между каждым набором данных. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | Проверить все данные, чтобы определить тип данных столбцов. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | Проверить, существует ли имя таблицы перед созданием. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getColumnTypeMap()](#getColumnTypeMap--) | Получает отображение типов столбцов для разных баз данных. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getCreateTable()](#getCreateTable--) | Указывает, экспортировать ли sql создания таблицы. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getExportArea()](#getExportArea--) | Получает диапазон экспорта. |
| [getExportAsString()](#getExportAsString--) | Указывает, экспортировать ли все данные как строковые значения. |
| [getIdName()](#getIdName--) | Получает имя столбца id. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getOperatorType()](#getOperatorType--) | Получает тип оператора sql. |
| [getPrimaryKey()](#getPrimaryKey--) | Представляет, какой столбец является первичным ключом таблицы данных. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSeparator()](#getSeparator--) | Получает символ‑разделитель sql‑скрипта. |
| [getSheetIndexes()](#getSheetIndexes--) | Представляет индексы экспортированных листов. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getStartId()](#getStartId--) | Получает начальный id. |
| [getTableName()](#getTableName--) | Получает имя таблицы. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hasHeaderRow()](#hasHeaderRow--) | Указывает, содержит ли диапазон строку заголовка. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | Вставлять пустую строку между каждым набором данных. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | Проверить все данные, чтобы определить тип данных столбцов. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | Проверить, существует ли имя таблицы перед созданием. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | Устанавливает отображение типов столбцов для разных баз данных. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | Указывает, экспортировать ли sql создания таблицы. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Устанавливает диапазон экспорта. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Указывает, экспортировать ли все данные как строковые значения. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Указывает, содержит ли диапазон строку заголовка. |
| [setIdName(String value)](#setIdName-java.lang.String-) | Устанавливает имя столбца id. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setOperatorType(int value)](#setOperatorType-int-) | Устанавливает тип оператора sql. |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | Представляет, какой столбец является первичным ключом таблицы данных. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setSeparator(char value)](#setSeparator-char-) | Устанавливает символ‑разделитель sql‑скрипта. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Представляет индексы экспортированных листов. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setStartId(int value)](#setStartId-int-) | Устанавливает начальный id. |
| [setTableName(String value)](#setTableName-java.lang.String-) | Устанавливает имя таблицы. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


Создаёт параметры для сохранения sql файла.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


Вставлять пустую строку между каждым набором данных.

**Remarks**

Если [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) равно '\\n', лучше установить это свойство в значение true, чтобы повысить читаемость.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Returns:**
java.lang.String
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


Проверить все данные, чтобы определить тип данных столбцов.

**Remarks**

Значение по умолчанию — false, мы проверяем только первую строку для повышения производительности. Если это свойство равно true и столбцы содержат смешанные типы значений, тип столбцов будет текстовым.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


Проверить, существует ли имя таблицы перед созданием.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Очищать книгу после сохранения файла.

**Returns:**
boolean
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


Получает отображение типов столбцов для разных баз данных.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


Указывает, экспортировать ли sql создания таблицы.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Получает диапазон экспорта.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Указывает, экспортировать ли все данные как строковые значения.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


Получает имя столбца id.

**Remarks**

Если это свойство установлено, столбец будет вставлен с автоматически увеличиваемым целочисленным значением.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


Получает тип оператора sql.

См. [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


Представляет, какой столбец является первичным ключом таблицы данных.

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Указывает, кэшировать ли последние данные диаграммы.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат сохраняемого файла.

Смотрите [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Получает символ‑разделитель sql‑скрипта.

**Remarks**

Только может быть ' ' или '\\n'. Если

**Returns:**
char
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Представляет индексы экспортированных листов.

**Returns:**
int[]
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Returns:**
boolean
### getStartId() {#getStartId--}
```
public int getStartId()
```


Получает начальный id.

**Remarks**

Работает только когда [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) установлен.

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


Получает имя таблицы.

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Указывает, содержит ли диапазон строку заголовка.

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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


Вставлять пустую строку между каждым набором данных.

**Remarks**

Если [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) равно '\\n', лучше установить это свойство в значение true, чтобы повысить читаемость.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Папка для временных файлов, которые могут использоваться в качестве кэша данных.

**Remarks**

Если папка не указана, значение по умолчанию для неё — [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Если её значение по умолчанию равно null или пусто, либо указано как null или пусто, то при сохранении книги кэш‑файл использоваться не будет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


Проверить все данные, чтобы определить тип данных столбцов.

**Remarks**

Значение по умолчанию — false, мы проверяем только первую строку для повышения производительности. Если это свойство равно true и столбцы содержат смешанные типы значений, тип столбцов будет текстовым.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


Проверить, существует ли имя таблицы перед созданием.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Очищать книгу после сохранения файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


Устанавливает отображение типов столбцов для разных баз данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


Указывает, экспортировать ли sql создания таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Устанавливает диапазон экспорта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Указывает, экспортировать ли все данные как строковые значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Указывает, содержит ли диапазон строку заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


Устанавливает имя столбца id.

**Remarks**

Если это свойство установлено, столбец будет вставлен с автоматически увеличиваемым целочисленным значением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


Устанавливает тип оператора sql.

См. [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


Представляет, какой столбец является первичным ключом таблицы данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Указывает, кэшировать ли последние данные диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Устанавливает символ‑разделитель sql‑скрипта.

**Remarks**

Только может быть ' ' или '\\n'. Если

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Представляет индексы экспортированных листов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Указывает, сортировать ли внешние определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Указывает, сортировать ли определённые имена перед сохранением файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


Устанавливает начальный id.

**Remarks**

Работает только когда [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) установлен.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


Устанавливает имя таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Указывает, следует ли обновлять настройки Smart Art. Значение по умолчанию — false.

**Remarks**

Влияет только после вызова метода Shape.GetResultOfSmartArt() и если кэшированные фигуры существуют в файле шаблона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Указывает, проверять ли объединённые ячейки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Устанавливает обратный вызов предупреждения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

