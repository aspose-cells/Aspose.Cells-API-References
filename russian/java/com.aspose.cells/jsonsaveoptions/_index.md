---
title: "JsonSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения рабочей книги в виде файла JSON."
type: docs
url: /ru/java/com.aspose.cells/jsonsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class JsonSaveOptions extends SaveOptions
```

Представляет параметры сохранения рабочей книги в виде файла JSON.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [JsonSaveOptions()](#JsonSaveOptions--) | Создает параметры для сохранения JSON‑файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--) | Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getExportArea()](#getExportArea--) | Получает диапазон экспорта. |
| [getExportAsString()](#getExportAsString--) | Экспортирует строковое значение ячеек в JSON. |
| [getExportEmptyCells()](#getExportEmptyCells--) | Указывает, экспортировать ли пустые ячейки как null. |
| [getExportHyperlinkType()](#getExportHyperlinkType--) | Представляет тип экспорта гиперссылки в JSON. |
| [getExportNestedStructure()](#getExportNestedStructure--) | Экспортируется как иерархическая структура JSON родитель‑ребёнок. |
| [getExportStylePool()](#getExportStylePool--) | Указывает, экспортировать стили коллективно или индивидуально для каждой ячейки. |
| [getIndent()](#getIndent--) | Указывает отступ. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSchemas()](#getSchemas--) | Исходная схема JSON для каждого листа. |
| [getSheetIndexes()](#getSheetIndexes--) | Представляет индексы экспортированных листов. |
| [getSkipEmptyRows()](#getSkipEmptyRows--) | Указывает, пропускать ли пустые строки. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getToExcelStruct()](#getToExcelStruct--) | Указывает, преобразовывать ли в структуру JSON файла Excel. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hasHeaderRow()](#hasHeaderRow--) | Указывает, содержит ли диапазон строку заголовка. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysExportAsJsonObject(boolean value)](#setAlwaysExportAsJsonObject-boolean-) | Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Устанавливает диапазон экспорта. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Экспортирует строковое значение ячеек в JSON. |
| [setExportEmptyCells(boolean value)](#setExportEmptyCells-boolean-) | Указывает, экспортировать ли пустые ячейки как null. |
| [setExportHyperlinkType(int value)](#setExportHyperlinkType-int-) | Представляет тип экспорта гиперссылки в JSON. |
| [setExportNestedStructure(boolean value)](#setExportNestedStructure-boolean-) | Экспортируется как иерархическая структура JSON родитель‑ребёнок. |
| [setExportStylePool(boolean value)](#setExportStylePool-boolean-) | Указывает, экспортировать стили коллективно или индивидуально для каждой ячейки. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Указывает, содержит ли диапазон строку заголовка. |
| [setIndent(String value)](#setIndent-java.lang.String-) | Указывает отступ. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setSchemas(String[] value)](#setSchemas-java.lang.String---) | Исходная схема JSON для каждого листа. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Представляет индексы экспортированных листов. |
| [setSkipEmptyRows(boolean value)](#setSkipEmptyRows-boolean-) | Указывает, пропускать ли пустые строки. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setToExcelStruct(boolean value)](#setToExcelStruct-boolean-) | Указывает, преобразовывать ли в структуру JSON файла Excel. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonSaveOptions() {#JsonSaveOptions--}
```
public JsonSaveOptions()
```


Создает параметры для сохранения JSON‑файла.

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
### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}
```
public boolean getAlwaysExportAsJsonObject()
```


Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист.

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
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

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


Экспортирует строковое значение ячеек в JSON.

**Returns:**
boolean
### getExportEmptyCells() {#getExportEmptyCells--}
```
public boolean getExportEmptyCells()
```


Указывает, экспортировать ли пустые ячейки как null.

**Returns:**
boolean
### getExportHyperlinkType() {#getExportHyperlinkType--}
```
public int getExportHyperlinkType()
```


Представляет тип экспорта гиперссылки в JSON.

Смотрите [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Значение по умолчанию — [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Returns:**
int
### getExportNestedStructure() {#getExportNestedStructure--}
```
public boolean getExportNestedStructure()
```


Экспортируется как иерархическая структура JSON родитель‑ребёнок.

**Remarks**

**Returns:**
boolean
### getExportStylePool() {#getExportStylePool--}
```
public boolean getExportStylePool()
```


Указывает, экспортировать стили коллективно или индивидуально для каждой ячейки.

**Returns:**
boolean
### getIndent() {#getIndent--}
```
public String getIndent()
```


Указывает отступ.

**Remarks**

Если отступ равен null или пуст, экспортированный JSON не форматируется.

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
### getSchemas() {#getSchemas--}
```
public String[] getSchemas()
```


Исходная схема JSON для каждого листа.

**Returns:**
java.lang.String[]
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Представляет индексы экспортированных листов.

**Returns:**
int[]
### getSkipEmptyRows() {#getSkipEmptyRows--}
```
public boolean getSkipEmptyRows()
```


Указывает, пропускать ли пустые строки.

**Returns:**
boolean
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
### getToExcelStruct() {#getToExcelStruct--}
```
public boolean getToExcelStruct()
```


Указывает, преобразовывать ли в структуру JSON файла Excel.

**Remarks**

Только для преобразования диапазона в JSON.

**Returns:**
boolean
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




### setAlwaysExportAsJsonObject(boolean value) {#setAlwaysExportAsJsonObject-boolean-}
```
public void setAlwaysExportAsJsonObject(boolean value)
```


Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист.

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

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32K. Когда вы вводите значение длиннее 32K, оно будет усечено.

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


Экспортирует строковое значение ячеек в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportEmptyCells(boolean value) {#setExportEmptyCells-boolean-}
```
public void setExportEmptyCells(boolean value)
```


Указывает, экспортировать ли пустые ячейки как null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportHyperlinkType(int value) {#setExportHyperlinkType-int-}
```
public void setExportHyperlinkType(int value)
```


Представляет тип экспорта гиперссылки в JSON.

Смотрите [JsonExportHyperlinkType](../../com.aspose.cells/jsonexporthyperlinktype).

**Remarks**

Значение по умолчанию — [JsonExportHyperlinkType.DISPLAY\_STRING](../../com.aspose.cells/jsonexporthyperlinktype\#DISPLAY-STRING);

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setExportNestedStructure(boolean value) {#setExportNestedStructure-boolean-}
```
public void setExportNestedStructure(boolean value)
```


Экспортируется как иерархическая структура JSON родитель‑ребёнок.

**Remarks**

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportStylePool(boolean value) {#setExportStylePool-boolean-}
```
public void setExportStylePool(boolean value)
```


Указывает, экспортировать стили коллективно или индивидуально для каждой ячейки.

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

### setIndent(String value) {#setIndent-java.lang.String-}
```
public void setIndent(String value)
```


Указывает отступ.

**Remarks**

Если отступ равен null или пуст, экспортированный JSON не форматируется.

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Указывает, кэшировать ли последние данные диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSchemas(String[] value) {#setSchemas-java.lang.String---}
```
public void setSchemas(String[] value)
```


Исходная схема JSON для каждого листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String[] |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Представляет индексы экспортированных листов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

### setSkipEmptyRows(boolean value) {#setSkipEmptyRows-boolean-}
```
public void setSkipEmptyRows(boolean value)
```


Указывает, пропускать ли пустые строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setToExcelStruct(boolean value) {#setToExcelStruct-boolean-}
```
public void setToExcelStruct(boolean value)
```


Указывает, преобразовывать ли в структуру JSON файла Excel.

**Remarks**

Только для преобразования диапазона в JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

