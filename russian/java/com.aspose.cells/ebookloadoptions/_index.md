---
title: "EbookLoadOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры при импорте файла электронного книги."
type: docs
url: /ru/java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

Представляет параметры при импорте файла электронного книги.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | Создаёт параметр для загрузки файла электронной книги. |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | Создаёт параметр загрузки файла электронной книги. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Каталог, в который будут сохраняться вложенные файлы. |
| [getAutoFilter()](#getAutoFilter--) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Указывает, следует ли автоматически подгонять столбцы и строки. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Получает параметры автоподгонки |
| [getCheckDataValid()](#getCheckDataValid--) | Проверьте, действительны ли данные в шаблонном файле. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в данные типа дата. |
| [getConvertFormulasData()](#getConvertFormulasData--) | Если true, преобразовывать строку в формулу, когда её значение начинается с символа '=', значение по умолчанию — false. |
| [getConvertNumericData()](#getConvertNumericData--) | Получает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Указывает, следует ли удалять лишние пробелы, когда текст переносит строки с помощью тега `<br>`. |
| [getDetectLaTeX()](#getDetectLaTeX--) | Указывает, следует ли обнаруживать формулы LaTeX в HTML‑файле. |
| [getEncoding()](#getEncoding--) | Получает кодировку по умолчанию. |
| [getFontConfigs()](#getFontConfigs--) | Получает отдельные конфигурации шрифтов. |
| [getHyperlinkLoadMode()](#getHyperlinkLoadMode--) | Указывает, как загружаются гиперссылки при загрузке HTML. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Получает монитор прерываний. |
| [getKeepPrecision()](#getKeepPrecision--) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [getLanguageCode()](#getLanguageCode--) | Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [getLoadFilter()](#getLoadFilter--) | Фильтр, определяющий способ загрузки данных. |
| [getLoadFormat()](#getLoadFormat--) | Получает формат загрузки. |
| [getLoadFormulas()](#getLoadFormulas--) | Указывает, импортировать ли формулы, если исходный HTML‑файл содержит формулы. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [getLocale()](#getLocale--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getMemorySetting()](#getMemorySetting--) | Получает режим памяти для загруженной рабочей книги. |
| [getParagrahLayoutMode()](#getParagrahLayoutMode--) | Указывает, как элементы HTML <p> отображаются при загрузке HTML. |
| [getParagraphLayoutMode()](#getParagraphLayoutMode--) | Указывает, как элементы HTML <p> отображаются при загрузке HTML. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Указывает, следует ли разбирать формулу при чтении файла. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [getPassword()](#getPassword--) | Получает пароль рабочей книги. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [getProgId()](#getProgId--) | Получает идентификатор программы, создавшей файл. |
| [getRegion()](#getRegion--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getStandardFont()](#getStandardFont--) | Устанавливает имя стандартного шрифта по умолчанию |
| [getStandardFontSize()](#getStandardFontSize--) | Устанавливает размер стандартного шрифта по умолчанию. |
| [getStreamProvider()](#getStreamProvider--) | Получает StreamProviderImportHtmlFile для импорта объектов. |
| [getSupportDivTag()](#getSupportDivTag--) | Указывает, поддерживается ли макет тега `<div>`, когда HTML‑файл содержит его. |
| [getTableLoadOptions()](#getTableLoadOptions--) | Получить экземпляр HtmlTableLoadOptionCollection |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hasFormula()](#hasFormula--) | Указывает, является ли текст формулой, если он начинается с "=". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Каталог, в который будут сохраняться вложенные файлы. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | Указывает, следует ли автоматически подгонять столбцы и строки. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Устанавливает параметры автоподгонки |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Проверьте, действительны ли данные в шаблонном файле. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в дату. |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | Если true, преобразовывать строку в формулу, когда её значение начинается с символа '=', значение по умолчанию — false. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Устанавливает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | Указывает, следует ли удалять лишние пробелы, когда текст переносит строки с помощью тега `<br>`. |
| [setDetectLaTeX(boolean value)](#setDetectLaTeX-boolean-) | Указывает, следует ли обнаруживать формулы LaTeX в HTML‑файле. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Устанавливает кодировку по умолчанию. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Устанавливает индивидуальные настройки шрифтов. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Указывает, является ли текст формулой, если он начинается с "=". |
| [setHyperlinkLoadMode(int value)](#setHyperlinkLoadMode-int-) | Указывает, как загружаются гиперссылки при загрузке HTML. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Устанавливает монитор прерываний. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Указывает, следует ли не разбирать строковое значение, если его длина составляет 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Фильтр, определяющий способ загрузки данных. |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | Указывает, импортировать ли формулы, если исходный HTML‑файл содержит формулы. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Устанавливает режим памяти для загруженного workbook. |
| [setPaperSize(int type)](#setPaperSize-int-) | Устанавливает размер бумаги по умолчанию для печати из настроек принтера по умолчанию. |
| [setParagrahLayoutMode(int value)](#setParagrahLayoutMode-int-) | Указывает, как элементы HTML <p> отображаются при загрузке HTML. |
| [setParagraphLayoutMode(int value)](#setParagraphLayoutMode-int-) | Указывает, как элементы HTML <p> отображаются при загрузке HTML. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Указывает, следует ли разбирать формулу при чтении файла. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [setRegion(int value)](#setRegion-int-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Устанавливает имя стандартного шрифта по умолчанию |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Устанавливает размер стандартного шрифта по умолчанию. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Устанавливает StreamProviderImportHtmlFile для импорта объектов. |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | Указывает, поддерживается ли макет тега `<div>`, когда HTML‑файл содержит его. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


Создаёт параметр для загрузки файла электронной книги.

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


Создаёт параметр загрузки файла электронной книги.

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Каталог, в который будут сохраняться вложенные файлы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство HtmlLoadOptions.StreamProvider. Это свойство будет удалено через 12 месяцев, начиная с декабря 2014 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Указывает, следует ли автоматически фильтровать данные при загрузке файлов.

**Remarks**

Иногда, хотя автотест (autofilter) установлен, соответствующие строки не скрываются в файле. Сейчас работает только для файлов SpreadSheetML.

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


Указывает, выполнять ли автоматическое подгонку столбцов и строк. Значение по умолчанию — false.

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
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


Если true, преобразовывать строку в формулу, когда её значение начинается с символа '=', значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство HtmlLoadOptions.HasFormula. Это свойство будет удалено через 12 месяцев, начиная с марта 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


Указывает, удалять ли лишние пробелы, когда текст переносит строки с помощью тега `<br>`. Значение по умолчанию — false.

**Returns:**
boolean
### getDetectLaTeX() {#getDetectLaTeX--}
```
public boolean getDetectLaTeX()
```


Указывает, обнаруживать ли LaTeX‑формулы в HTML‑файле. Значение по умолчанию — false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Получает кодировку по умолчанию. Применяется только для CSV‑файлов.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Получает индивидуальные настройки шрифтов. Работает только с [Workbook](../../com.aspose.cells/workbook), который использует эти [LoadOptions](../../com.aspose.cells/loadoptions) для загрузки.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHyperlinkLoadMode() {#getHyperlinkLoadMode--}
```
public int getHyperlinkLoadMode()
```


Указывает, как загружаются гиперссылки при загрузке HTML.

См. [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

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
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


Указывает, импортировать ли формулы, если исходный HTML‑файл содержит формулы.

**Returns:**
boolean
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
### getParagrahLayoutMode() {#getParagrahLayoutMode--}
```
public int getParagrahLayoutMode()
```


Указывает, как отображаются элементы HTML <p> при загрузке HTML. Значение по умолчанию — [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

См. [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство HtmlLoadOptions.ParagraphLayoutMode. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getParagraphLayoutMode() {#getParagraphLayoutMode--}
```
public int getParagraphLayoutMode()
```


Указывает, как отображаются элементы HTML <p> при загрузке HTML. Значение по умолчанию — [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

См. [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

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
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

**Remarks**

После загрузки книги из шаблонного файла с этой опцией, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) будет установлена в то же значение, что и это свойство.

**Returns:**
boolean
### getProgId() {#getProgId--}
```
public String getProgId()
```


Возвращает идентификатор программы, создавшей файл. Только для файлов MHT.

**Returns:**
java.lang.String
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
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Получает StreamProviderImportHtmlFile для импорта объектов.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


Указывает, поддерживается ли разметка тега `<div>`, когда HTML‑файл содержит его. Значение по умолчанию — false.

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


Получить экземпляр HtmlTableLoadOptionCollection

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Каталог, в который будут сохраняться вложенные файлы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство HtmlLoadOptions.StreamProvider. Это свойство будет удалено через 12 месяцев, начиная с декабря 2014 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


Указывает, выполнять ли автоматическое подгонку столбцов и строк. Значение по умолчанию — false.

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

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


Если true, преобразовывать строку в формулу, когда её значение начинается с символа '=', значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство HtmlLoadOptions.HasFormula. Это свойство будет удалено через 12 месяцев, начиная с марта 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


Указывает, удалять ли лишние пробелы, когда текст переносит строки с помощью тега `<br>`. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDetectLaTeX(boolean value) {#setDetectLaTeX-boolean-}
```
public void setDetectLaTeX(boolean value)
```


Указывает, обнаруживать ли LaTeX‑формулы в HTML‑файле. Значение по умолчанию — false.

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

### setHyperlinkLoadMode(int value) {#setHyperlinkLoadMode-int-}
```
public void setHyperlinkLoadMode(int value)
```


Указывает, как загружаются гиперссылки при загрузке HTML.

См. [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

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

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


Указывает, импортировать ли формулы, если исходный HTML‑файл содержит формулы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setParagrahLayoutMode(int value) {#setParagrahLayoutMode-int-}
```
public void setParagrahLayoutMode(int value)
```


Указывает, как отображаются элементы HTML <p> при загрузке HTML. Значение по умолчанию — [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

См. [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство HtmlLoadOptions.ParagraphLayoutMode. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setParagraphLayoutMode(int value) {#setParagraphLayoutMode-int-}
```
public void setParagraphLayoutMode(int value)
```


Указывает, как отображаются элементы HTML <p> при загрузке HTML. Значение по умолчанию — [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

См. [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Устанавливает StreamProviderImportHtmlFile для импорта объектов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


Указывает, поддерживается ли разметка тега `<div>`, когда HTML‑файл содержит его. Значение по умолчанию — false.

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

