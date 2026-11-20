---
title: "TxtSaveOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры сохранения для формата csv/разделённого табуляцией/других текстовых форматов."
type: docs
url: /ru/java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

Представляет параметры сохранения для формата csv/разделённого табуляцией/других текстовых форматов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Создаёт параметры сохранения текстового файла. |
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Создаёт параметры сохранения текстового файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Указывает, следует ли всегда добавлять '\\"' для каждого поля. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Очищать книгу после сохранения файла. |
| [getCreateDirectory()](#getCreateDirectory--) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [getEncoding()](#getEncoding--) | Получает кодировку по умолчанию. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [getExportAllSheets()](#getExportAllSheets--) | Указывает, экспортировать ли все листы в текстовый файл. |
| [getExportArea()](#getExportArea--) | Диапазон ячеек для экспорта. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) возвращает true. |
| [getFormatStrategy()](#getFormatStrategy--) | Получает стратегию форматирования при экспорте значения ячейки как строки. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Указывает, следует ли выводить разделители для пустой строки. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Поставщик данных для сохранения рабочей книги в лёгком режиме. |
| [getMergeAreas()](#getMergeAreas--) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [getQuoteType()](#getQuoteType--) | Получает способ кавычивания значений в экспортированном текстовом файле. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Указывает, кэшировать ли последние данные диаграммы. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат сохраняемого файла. |
| [getSeparator()](#getSeparator--) | Получает символ-разделитель текстового файла. |
| [getSeparatorString()](#getSeparatorString--) | Получает строковое значение в качестве разделителя. |
| [getSortExternalNames()](#getSortExternalNames--) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [getSortNames()](#getSortNames--) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Указывает, следует ли обрезать завершающие пустые ячейки в строке. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Указывает, обновлять ли настройки SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Указывает, следует ли всегда добавлять '\\"' для каждого поля. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Папка для временных файлов, которые могут использоваться в качестве кэша данных. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setClearData(boolean value)](#setClearData-boolean-) | Очищать книгу после сохранения файла. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Устанавливает кодировку по умолчанию. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Указывает, экспортировать ли все листы в текстовый файл. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Диапазон ячеек для экспорта. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) возвращает true. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Устанавливает стратегию форматирования при экспорте значения ячейки как строки. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Указывает, следует ли выводить разделители для пустой строки. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Поставщик данных для сохранения рабочей книги в лёгком режиме. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла. |
| [setQuoteType(int value)](#setQuoteType-int-) | Устанавливает способ кавычивания значений в экспортированном текстовом файле. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Указывает, кэшировать ли последние данные диаграммы. |
| [setSeparator(char value)](#setSeparator-char-) | Устанавливает символ-разделитель текстового файла. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Устанавливает строковое значение в качестве разделителя. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Указывает, сортировать ли внешние определённые имена перед сохранением файла. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Указывает, сортировать ли определённые имена перед сохранением файла. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Указывает, следует ли обрезать завершающие пустые ячейки в строке. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Указывает, обновлять ли настройки SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Указывает, проверять ли объединённые ячейки перед сохранением файла. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Создаёт параметры сохранения текстового файла.

### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```


Создаёт параметры сохранения текстового файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Формат файла. Должен быть [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV) или [SaveFormat.TSV](../../com.aspose.cells/saveformat\\#TSV), иначе формат сохранения будет автоматически установлен как [SaveFormat.CSV](../../com.aspose.cells/saveformat\\#CSV). |

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
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Указывает, следует ли всегда добавлять '\\"' для каждого поля. Если true, все значения будут заключены в кавычки; если false, значения будут заключаться в кавычки только при необходимости (например, когда значения содержат специальные символы, такие как '\\"', '\\\\n' или разделитель). По умолчанию false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство QuoteType. Это свойство будет удалено через 12 месяцев, начиная с августа 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Получает кодировку по умолчанию.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.

**Remarks**

Только для файлов .xls, .xlsx, .xlsb и .xlsm.

**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Указывает, экспортировать ли все листы в текстовый файл. Если false, будет экспортирован только активный лист, как в MS Excel.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Диапазон ячеек для экспорта.

**Remarks**

Если экспортированная область указана, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) не будет иметь эффекта.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) имеет значение true. По умолчанию — false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Получает стратегию форматирования при экспорте значения ячейки как строки.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию — false, поэтому по умолчанию содержимое пустой строки будет пустым.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Поставщик данных для сохранения рабочей книги в лёгком режиме.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Указывает, следует ли объединять области условного форматирования и проверки перед сохранением файла.

**Remarks**

Значение по умолчанию — false.

**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Получает способ кавычивания значений в экспортированном текстовом файле.

Смотрите [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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


Получает символ-разделитель текстового файла.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Получает строковое значение в качестве разделителя.

**Returns:**
java.lang.String
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
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. По умолчанию — true.

**Remarks**

То же правило, что и в MS Excel: строка/столбец не считается пустым, если у него есть пользовательский стиль, даже если в нём нет данных ячеек. При сохранении в режиме LightCells эта опция не действует. Пользователь должен управлять диапазоном вывода с помощью реализации [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) или указав [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Указывает, следует ли обрезать завершающие пустые ячейки в строке. По умолчанию — false.

**Remarks**

При сохранении в режиме LightCells и если [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) не указана, эта опция не действует, и строка будет расширена до последней ячейки, предоставленной реализацией [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Указывает, следует ли всегда добавлять '\\"' для каждого поля. Если true, все значения будут заключены в кавычки; если false, значения будут заключаться в кавычки только при необходимости (например, когда значения содержат специальные символы, такие как '\\"', '\\\\n' или разделитель). По умолчанию false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство QuoteType. Это свойство будет удалено через 12 месяцев, начиная с августа 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Устанавливает кодировку по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Указывает, экспортировать ли все листы в текстовый файл. Если false, будет экспортирован только активный лист, как в MS Excel.

**Remarks**

Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Диапазон ячеек для экспорта.

**Remarks**

Если экспортированная область указана, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) не будет иметь эффекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Указывает, следует ли экспортировать знак одинарной кавычки как часть значения ячейки, когда [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) имеет значение true. По умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Устанавливает стратегию форматирования при экспорте значения ячейки как строки.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию — false, поэтому по умолчанию содержимое пустой строки будет пустым.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Поставщик данных для сохранения рабочей книги в лёгком режиме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Устанавливает способ кавычивания значений в экспортированном текстовом файле.

Смотрите [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).

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


Устанавливает символ-разделитель текстового файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Устанавливает строковое значение в качестве разделителя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


Указывает, следует ли обрезать ведущие пустые строки и столбцы, как делает MS Excel. По умолчанию — true.

**Remarks**

То же правило, что и в MS Excel: строка/столбец не считается пустым, если у него есть пользовательский стиль, даже если в нём нет данных ячеек. При сохранении в режиме LightCells эта опция не действует. Пользователь должен управлять диапазоном вывода с помощью реализации [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) или указав [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Указывает, следует ли обрезать завершающие пустые ячейки в строке. По умолчанию — false.

**Remarks**

При сохранении в режиме LightCells и если [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) не указана, эта опция не действует, и строка будет расширена до последней ячейки, предоставленной реализацией [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--).

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

