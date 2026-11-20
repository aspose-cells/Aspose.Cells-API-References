---
title: "TxtLoadOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры загрузки текстового файла."
type: docs
url: /ru/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Представляет параметры загрузки текстового файла.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Создаёт параметры для загрузки текстового файла. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Создаёт параметры для загрузки текстового файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Получает параметры автоподгонки |
| [getCheckDataValid()](#getCheckDataValid--) | Проверьте, действительны ли данные в шаблонном файле. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в данные типа дата. |
| [getConvertNumericData()](#getConvertNumericData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [getEncoding()](#getEncoding--) | Получает кодировку по умолчанию. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Расширяет ли данные на следующий лист, когда количество строк или столбцов данных превышает лимит. |
| [getFontConfigs()](#getFontConfigs--) | Получает отдельные конфигурации шрифтов. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | Количество столбцов заголовка, которые будут повторяться для расширенных листов. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | Количество строк заголовка, которые будут повторяться для расширенных листов. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Получает монитор прерываний. |
| [getKeepPrecision()](#getKeepPrecision--) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [getLanguageCode()](#getLanguageCode--) | Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [getLoadFilter()](#getLoadFilter--) | Фильтр, определяющий способ загрузки данных. |
| [getLoadFormat()](#getLoadFormat--) | Получает формат загрузки. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [getLocale()](#getLocale--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getMaxColumnCount()](#getMaxColumnCount--) | Максимальное количество столбцов, которые могут быть импортированы для одного листа. |
| [getMaxRowCount()](#getMaxRowCount--) | Максимальное количество строк, импортируемых в один лист. |
| [getMemorySetting()](#getMemorySetting--) | Получает режим памяти для загруженной рабочей книги. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Указывает, следует ли разбирать формулу при чтении файла. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [getPassword()](#getPassword--) | Получает пароль рабочей книги. |
| [getPreferredParsers()](#getPreferredParsers--) | Получает предпочтительные парсеры значений для загрузки текстового файла. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [getRegion()](#getRegion--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getSeparator()](#getSeparator--) | Получает символьный разделитель текстового файла. |
| [getSeparatorString()](#getSeparatorString--) | Получает строковое значение в качестве разделителя. |
| [getStandardFont()](#getStandardFont--) | Устанавливает имя стандартного шрифта по умолчанию |
| [getStandardFontSize()](#getStandardFontSize--) | Устанавливает размер стандартного шрифта по умолчанию. |
| [getTextQualifier()](#getTextQualifier--) | Указывает текстовый квалификатор для значений ячеек. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hasFormula()](#hasFormula--) | Указывает, является ли текст формулой, если он начинается с "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Есть ли текстовый квалификатор для значения ячейки. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True означает, что файл содержит несколько кодировок. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Устанавливает параметры автоподгонки |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Проверьте, действительны ли данные в шаблонном файле. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в дату. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Устанавливает кодировку по умолчанию. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Расширяет ли данные на следующий лист, когда количество строк или столбцов данных превышает лимит. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Устанавливает индивидуальные настройки шрифтов. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Указывает, является ли текст формулой, если он начинается с "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Есть ли текстовый квалификатор для значения ячейки. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | Количество столбцов заголовка, которые будут повторяться для расширенных листов. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | Количество строк заголовка, которые будут повторяться для расширенных листов. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Устанавливает монитор прерываний. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Фильтр, определяющий способ загрузки данных. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | Максимальное количество столбцов, которые могут быть импортированы для одного листа. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | Максимальное количество строк, импортируемых в один лист. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Устанавливает режим памяти для загруженного workbook. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True означает, что файл содержит несколько кодировок. |
| [setPaperSize(int type)](#setPaperSize-int-) | Устанавливает размер бумаги по умолчанию для печати из настроек принтера по умолчанию. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Указывает, следует ли разбирать формулу при чтении файла. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для workbook. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Устанавливает предпочтительные парсеры значений для загрузки текстового файла. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [setRegion(int value)](#setRegion-int-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setSeparator(char value)](#setSeparator-char-) | Устанавливает символьный разделитель текстового файла. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Устанавливает строковое значение в качестве разделителя. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Устанавливает имя стандартного шрифта по умолчанию |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Устанавливает размер стандартного шрифта по умолчанию. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Указывает текстовый квалификатор для значений ячеек. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Создаёт параметры для загрузки текстового файла.

**Remarks**

Тип файла по умолчанию для загрузки — CSV.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Создаёт параметры для загрузки текстового файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Формат загрузки |

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

**Remarks**

Иногда, хотя автотест (autofilter) установлен, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Получает параметры автоподгонки

**Remarks**

Только для файлов xlsx, spreadsheetML в данный момент.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Проверьте, действительны ли данные в шаблонном файле.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недопустимо для формата файла Excel, позже не следует сохранять workbook в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Получает значение, указывающее, преобразуется ли строка в текстовом файле в дату. Значение по умолчанию — true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Получает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Получает настройки стиля по умолчанию для инициализации стилей рабочей книги

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Получает кодировку по умолчанию. Применяется только для CSV‑файлов.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Определяет, расширять ли данные на следующий лист, когда количество строк или столбцов превышает предел. По умолчанию — false.

**Remarks**

Если это свойство истинно, дополнительные данные будут помещены на следующий лист после текущего (если текущий лист последний, будет добавлен новый лист в текущую книгу). Если это свойство ложно, данные, превышающие предел, будут игнорироваться.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Получает индивидуальные настройки шрифтов. Работает только с [Workbook](../../com.aspose.cells/workbook), который использует эти [LoadOptions](../../com.aspose.cells/loadoptions) для загрузки.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


Количество столбцов заголовка, которые будут повторяться для расширенных листов.

**Remarks**

Столбцы заголовков, указанные этим свойством, будут дублироваться для расширенных листов. Это свойство действует только когда [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) истинно.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


Количество строк заголовка, которые будут повторяться для расширенных листов.

**Remarks**

Строки заголовков, указанные этим свойством, будут дублироваться для расширенных листов. Это свойство действует только когда [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) истинно.

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Игнорировать данные, которые не печатаются при прямой печати файла

**Remarks**

Только для файлов xlsx.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Указывает, следует ли игнорировать бесполезные фигуры.

**Remarks**

Работает только с файлами xlsx, xlsb и xlsm. В некоторых файлах присутствует множество перекрывающихся одинаковых фигур, которые бесполезны; мы можем игнорировать их при загрузке файлов.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Получает монитор прерываний.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Указывает, следует ли не разбирать строковое значение, если его длина составляет 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

**Remarks**

В сценариях, когда пользователю необходимо только прочитать часть содержимого шаблонного файла и не требуется сохранять workbook обратно, установка этого свойства в false может повысить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Обработчик данных для обработки данных ячеек при чтении шаблонного файла.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Фильтр, определяющий способ загрузки данных.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Получает формат загрузки.

Смотрите [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время.

См. [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Получает региональные настройки, используемые для загружаемой рабочей книги.

**Remarks**

Это свойство имеет тот же эффект, что и [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) при установке региональных настроек.

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


Максимальное количество столбцов, которые могут быть импортированы для одного листа.

**Remarks**

Столбцы, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Это количество включает столбцы заголовков ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Максимальное значение — ограничение столбцов соответствующего формата файла, например для файла xlsx это 16384. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


Максимальное количество строк, импортируемых в один лист.

**Remarks**

Строки, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Это количество включает строки заголовков ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Максимальное допустимое значение — ограничение строк соответствующего формата файла, например для файла xlsx это 1048576. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Получает режим памяти для загруженной рабочей книги.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Для получения более подробной информации о режиме памяти, пожалуйста, смотрите [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Указывает, следует ли разбирать формулу при чтении файла.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm и Xlsm, поскольку формулы в этих файлах хранятся в виде строковой формулы.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm, Xlsm и xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Получает пароль рабочей книги.

**Returns:**
java.lang.String
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Получает предпочтительные парсеры значений для загрузки текстового файла.

**Remarks**

parsers[0] — парсер, который будет использоваться для первого столбца в файле шаблона текста, parsers[1] — парсер для второго столбца, … и т.д. Последний (parsers[parsers.length-1]) будет использоваться для всех остальных столбцов, начиная с parsers.length-1. Если элемент равен null, соответствующий столбец будет обрабатываться парсером по умолчанию Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

После загрузки книги из шаблонного файла с этой опцией, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) будет установлена в то же значение, что и это свойство.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Получает региональные настройки, используемые для загружаемой рабочей книги.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Региональные настройки могут использоваться для инициализации некоторых функций книги, таких как шрифты, темы и т.д. Для текстовых форматов файлов, таких как CSV, HTML, ..., региональная настройка также будет использоваться для определения форматов чисел и преобразования текстовых значений в числовые или datetime‑значения ячеек. Эта настройка будет сохранена для созданной позже книги, то есть [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) книги будет использовать тот же регион, что и это свойство.

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Получает символьный разделитель текстового файла.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Получает строковое значение в качестве разделителя.

**Returns:**
java.lang.String
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Устанавливает имя стандартного шрифта по умолчанию

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Устанавливает размер стандартного шрифта по умолчанию.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '\"'.

**Remarks**

При установке этого свойства [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) автоматически станет истинным.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Определяет, следует ли рассматривать последовательные разделители как один.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. По умолчанию — true. Если false, начальный одинарный апостроф будет удалён из значения соответствующей ячейки, и для ячейки будет установлено значение true у [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--).

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Получает обратный вызов предупреждения.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Указывает, является ли текст формулой, если он начинается с "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Есть ли текстовый квалификатор для значения ячейки. По умолчанию — true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True означает, что файл содержит несколько кодировок.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

**Remarks**

Иногда, хотя автотест (autofilter) установлен, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Устанавливает параметры автоподгонки

**Remarks**

Только для файлов xlsx, spreadsheetML в данный момент.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Проверьте, действительны ли данные в шаблонном файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недопустимо для формата файла Excel, позже не следует сохранять workbook в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Устанавливает кодировку по умолчанию. Применяется только для файлов csv.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Определяет, расширять ли данные на следующий лист, когда количество строк или столбцов превышает предел. По умолчанию — false.

**Remarks**

Если это свойство истинно, дополнительные данные будут помещены на следующий лист после текущего (если текущий лист последний, будет добавлен новый лист в текущую книгу). Если это свойство ложно, данные, превышающие предел, будут игнорироваться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Устанавливает индивидуальные конфигурации шрифтов. Работает только с [Workbook](../../com.aspose.cells/workbook), который использует эти [LoadOptions](../../com.aspose.cells/loadoptions) для загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Указывает, является ли текст формулой, если он начинается с "=".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Есть ли текстовый квалификатор для значения ячейки. По умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


Количество столбцов заголовка, которые будут повторяться для расширенных листов.

**Remarks**

Столбцы заголовков, указанные этим свойством, будут дублироваться для расширенных листов. Это свойство действует только когда [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) истинно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


Количество строк заголовка, которые будут повторяться для расширенных листов.

**Remarks**

Строки заголовков, указанные этим свойством, будут дублироваться для расширенных листов. Это свойство действует только когда [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) истинно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Игнорировать данные, которые не печатаются при прямой печати файла

**Remarks**

Только для файлов xlsx.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Указывает, следует ли игнорировать бесполезные фигуры.

**Remarks**

Работает только с файлами xlsx, xlsb и xlsm. В некоторых файлах присутствует множество перекрывающихся одинаковых фигур, которые бесполезны; мы можем игнорировать их при загрузке файлов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Устанавливает монитор прерываний.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Указывает, следует ли не разбирать строковое значение, если его длина составляет 15.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

**Remarks**

В сценариях, когда пользователю необходимо только прочитать часть содержимого шаблонного файла и не требуется сохранять workbook обратно, установка этого свойства в false может повысить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Обработчик данных для обработки данных ячеек при чтении шаблонного файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Фильтр, определяющий способ загрузки данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время.

См. [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Устанавливает региональные настройки, используемые для загружаемого Workbook.

**Remarks**

Это свойство имеет тот же эффект, что и [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) при установке региональных настроек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


Максимальное количество столбцов, которые могут быть импортированы для одного листа.

**Remarks**

Столбцы, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Это количество включает столбцы заголовков ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Максимальное значение — ограничение столбцов соответствующего формата файла, например для файла xlsx это 16384. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


Максимальное количество строк, импортируемых в один лист.

**Remarks**

Строки, превышающие этот предел, будут игнорироваться или переноситься на следующий лист в соответствии с [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Это количество включает строки заголовков ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Максимальное допустимое значение — ограничение строк соответствующего формата файла, например для файла xlsx это 1048576. Если это свойство не указано или указанное значение не положительно, будет использовано максимальное ограничение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Устанавливает режим памяти для загруженного workbook.

Смотрите [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Для получения более подробной информации о режиме памяти, пожалуйста, смотрите [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True означает, что файл содержит несколько кодировок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Устанавливает размер бумаги по умолчанию для печати из настроек принтера по умолчанию.

**Remarks**

Если настройка размера бумаги отсутствует, MS Excel будет использовать настройки принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). Размер бумаги по умолчанию. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Указывает, следует ли разбирать формулу при чтении файла.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm и Xlsm, поскольку формулы в этих файлах хранятся в виде строковой формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.

**Remarks**

Применяется только к файлам Excel Xlsx, Xltx, Xltm, Xlsm и xlsb.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Устанавливает пароль для workbook.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Устанавливает предпочтительные парсеры значений для загрузки текстового файла.

**Remarks**

parsers[0] — парсер, который будет использоваться для первого столбца в файле шаблона текста, parsers[1] — парсер для второго столбца, … и т.д. Последний (parsers[parsers.length-1]) будет использоваться для всех остальных столбцов, начиная с parsers.length-1. Если элемент равен null, соответствующий столбец будет обрабатываться парсером по умолчанию Aspose.Cells.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

После загрузки книги из шаблонного файла с этой опцией, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) будет установлена в то же значение, что и это свойство.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Устанавливает региональные настройки, используемые для загружаемого Workbook.

Смотрите [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Региональные настройки могут использоваться для инициализации некоторых функций книги, таких как шрифты, темы и т.д. Для текстовых форматов файлов, таких как CSV, HTML, ..., региональная настройка также будет использоваться для определения форматов чисел и преобразования текстовых значений в числовые или datetime‑значения ячеек. Эта настройка будет сохранена для созданной позже книги, то есть [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) книги будет использовать тот же регион, что и это свойство.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Устанавливает символьный разделитель текстового файла.

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

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Устанавливает имя стандартного шрифта по умолчанию

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Устанавливает размер стандартного шрифта по умолчанию.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '\"'.

**Remarks**

При установке этого свойства [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) автоматически станет истинным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Определяет, следует ли рассматривать последовательные разделители как один.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. По умолчанию — true. Если false, начальный одинарный апостроф будет удалён из значения соответствующей ячейки, и для ячейки будет установлено значение true у [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--).

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

