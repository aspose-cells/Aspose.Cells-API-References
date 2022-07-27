---
title: HtmlLoadOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры при импорте html-файла.
type: docs
weight: 3730
url: /ru/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Представляет параметры при импорте html-файла.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions#constructor)() | Создает опции загрузки файла. |
| [HtmlLoadOptions](htmlloadoptions#constructor_1)(LoadFormat) | Создает опции загрузки файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Указывает, выполняется ли автоматическая фильтрация данных при загрузке файлов. |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows) { get; set; } | Указывает, будут ли автоматически подбираться столбцы и строки. Значение по умолчанию — false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Получает и устанавливает параметры автоматической установки |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Проверить правильность данных в файле шаблона. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками. Например, excel не позволяет вводить строковое значение длиннее 32 КБ. имеет значение true, вы получите исключение. Если это свойство имеет значение false, мы примем введенное вами строковое значение в качестве значения ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако, если вы установили такое значение, которое недопустимо для формата файла Excel, вам не следует сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata) { get; set; } | если true, преобразовать строку в формулу, когда строковое значение начинается с символа '=', значение по умолчанию - false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Получает или задает информацию о культуре системы на момент загрузки файла. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces) { get; set; } | Указывает, следует ли удалять лишние пробелы, когда текст переносит строки с помощью тега &lt;br&gt;. Значение по умолчанию — false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Получает и задает кодировку по умолчанию. Применяется только для CSV-файла. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Получает и устанавливает отдельные конфигурации шрифтов. Работает только для[`Workbook`](../workbook) который использует это[`LoadOptions`](../loadoptions) для загрузки.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Игнорировать данные, которые не печатаются, при прямой печати файла |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Получает и устанавливает монитор прерываний. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Указывает, не анализировать ли строковое значение, если длина равна 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Сохранять ли непроанализированные данные в памяти для книги, когда она загружается из файла шаблона. Значение по умолчанию — true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в которой сохранен файл. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Обработчик данных для обработки данных ячеек при чтении файла шаблона. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Фильтр для обозначения способа загрузки данных. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Получает формат загрузки. |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas) { get; set; } | Указывает, нужно ли импортировать формулы, если исходный html-файл содержит формулы |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Указывает стратегию применения стиля для проанализированных значений при преобразовании строкового значения в число или дату и время. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Получает или задает параметры использования памяти. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Указывает, выполняется ли разбор формулы при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Указывает, анализируются ли сводные кэшированные записи при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Получает и устанавливает пароль книги. |
| [ProgId](../../aspose.cells/htmlloadoptions/progid) { get; } | Получает идентификатор программы создания файла. Только для файлов MHT. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Получает или задает региональные параметры системы на основе CountryCode на момент загрузки файла. |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider) { get; set; } | Получает или задает StreamProviderImportHtmlFile для импорта объектов. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag) { get; set; } | Указывает, поддерживается ли макет тега &lt;div&gt;, когда html-файл содержит теги &lt;div&gt;. Значение по умолчанию — false. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Устанавливает размер бумаги для печати по умолчанию из настроек принтера по умолчанию. |

### Смотрите также

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
