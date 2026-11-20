---
title: "JsonLoadOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры загрузки файлов JSON"
type: docs
url: /ru/java/com.aspose.cells/jsonloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class JsonLoadOptions extends LoadOptions
```

Представляет параметры загрузки файлов JSON
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [JsonLoadOptions()](#JsonLoadOptions--) | Создает параметры загрузки файла. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Получает параметры автоподгонки |
| [getCheckDataValid()](#getCheckDataValid--) | Проверьте, действительны ли данные в шаблонном файле. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [getClass()](#getClass--) |  |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [getFontConfigs()](#getFontConfigs--) | Получает отдельные конфигурации шрифтов. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Получает монитор прерываний. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [getKeptSchema()](#getKeptSchema--) | Указывает, сохраняется ли схема этого JSON. |
| [getLanguageCode()](#getLanguageCode--) | Получает язык пользовательского интерфейса версии рабочей книги, основанный на CountryCode, в котором файл был сохранён. |
| [getLayoutOptions()](#getLayoutOptions--) | Параметры импорта JSON. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [getLoadFilter()](#getLoadFilter--) | Фильтр, определяющий способ загрузки данных. |
| [getLoadFormat()](#getLoadFormat--) | Получает формат загрузки. |
| [getLocale()](#getLocale--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getMemorySetting()](#getMemorySetting--) | Получает режим памяти для загруженной рабочей книги. |
| [getMultipleWorksheets()](#getMultipleWorksheets--) | Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Указывает, следует ли разбирать формулу при чтении файла. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [getPassword()](#getPassword--) | Получает пароль рабочей книги. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [getRegion()](#getRegion--) | Получает региональные настройки, используемые для загружаемой рабочей книги. |
| [getStandardFont()](#getStandardFont--) | Устанавливает имя стандартного шрифта по умолчанию |
| [getStandardFontSize()](#getStandardFontSize--) | Устанавливает размер стандартного шрифта по умолчанию. |
| [getStartCell()](#getStartCell--) | Получает начальную ячейку. |
| [getWarningCallback()](#getWarningCallback--) | Получает обратный вызов предупреждения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Устанавливает параметры автоподгонки |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Проверьте, действительны ли данные в шаблонном файле. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Устанавливает индивидуальные настройки шрифтов. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Игнорировать данные, которые не печатаются при прямой печати файла |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Указывает, следует ли игнорировать бесполезные фигуры. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Устанавливает монитор прерываний. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Сохранять ли неразобранные данные в памяти для рабочей книги при загрузке из шаблонного файла. |
| [setKeptSchema(boolean value)](#setKeptSchema-boolean-) | Указывает, сохраняется ли схема этого JSON. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Устанавливает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [setLayoutOptions(JsonLayoutOptions value)](#setLayoutOptions-com.aspose.cells.JsonLayoutOptions-) | Параметры импорта JSON. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Фильтр, определяющий способ загрузки данных. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Устанавливает режим памяти для загруженного workbook. |
| [setMultipleWorksheets(boolean value)](#setMultipleWorksheets-boolean-) | Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами. |
| [setPaperSize(int type)](#setPaperSize-int-) | Устанавливает размер бумаги по умолчанию для печати из настроек принтера по умолчанию. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Указывает, следует ли разбирать формулу при чтении файла. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Устанавливает пароль для workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Указывает, следует ли сохранять пробелы и переводы строк, вставленные между токенами формулы при получении и установке формул. |
| [setRegion(int value)](#setRegion-int-) | Устанавливает региональные настройки, используемые для загружаемого Workbook. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Устанавливает имя стандартного шрифта по умолчанию |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Устанавливает размер стандартного шрифта по умолчанию. |
| [setStartCell(String value)](#setStartCell-java.lang.String-) | Устанавливает начальную ячейку. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Устанавливает обратный вызов предупреждения. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JsonLoadOptions() {#JsonLoadOptions--}
```
public JsonLoadOptions()
```


Создает параметры загрузки файла.

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
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Получает настройки стиля по умолчанию для инициализации стилей рабочей книги

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Получает индивидуальные настройки шрифтов. Работает только с [Workbook](../../com.aspose.cells/workbook), который использует эти [LoadOptions](../../com.aspose.cells/loadoptions) для загрузки.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
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
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.

**Remarks**

В сценариях, когда пользователю необходимо только прочитать часть содержимого шаблонного файла и не требуется сохранять workbook обратно, установка этого свойства в false может повысить производительность, особенно при совместном использовании с некоторыми типами LoadFilter,

**Returns:**
boolean
### getKeptSchema() {#getKeptSchema--}
```
public boolean getKeptSchema()
```


Указывает, сохраняется ли схема этого JSON.

**Remarks**

Иногда мы сохраняем файл в JSON после загрузки JSON-файла.

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
### getLayoutOptions() {#getLayoutOptions--}
```
public JsonLayoutOptions getLayoutOptions()
```


Параметры импорта JSON.

**Returns:**
[JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions)
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
### getMultipleWorksheets() {#getMultipleWorksheets--}
```
public boolean getMultipleWorksheets()
```


Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами.

**Returns:**
boolean
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
### getStartCell() {#getStartCell--}
```
public String getStartCell()
```


Получает начальную ячейку.

**Returns:**
java.lang.String
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

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Устанавливает индивидуальные конфигурации шрифтов. Работает только с [Workbook](../../com.aspose.cells/workbook), который использует эти [LoadOptions](../../com.aspose.cells/loadoptions) для загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setKeptSchema(boolean value) {#setKeptSchema-boolean-}
```
public void setKeptSchema(boolean value)
```


Указывает, сохраняется ли схема этого JSON.

**Remarks**

Иногда мы сохраняем файл в JSON после загрузки JSON-файла.

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

### setLayoutOptions(JsonLayoutOptions value) {#setLayoutOptions-com.aspose.cells.JsonLayoutOptions-}
```
public void setLayoutOptions(JsonLayoutOptions value)
```


Параметры импорта JSON.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [JsonLayoutOptions](../../com.aspose.cells/jsonlayoutoptions) |  |

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

### setMultipleWorksheets(boolean value) {#setMultipleWorksheets-boolean-}
```
public void setMultipleWorksheets(boolean value)
```


Указывает, импортировать ли каждый атрибут объекта JsonObject как отдельный лист, когда все дочерние узлы являются массивами.

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

### setStartCell(String value) {#setStartCell-java.lang.String-}
```
public void setStartCell(String value)
```


Устанавливает начальную ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

