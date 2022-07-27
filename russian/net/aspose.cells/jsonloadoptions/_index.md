---
title: JsonLoadOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры загрузки файлов json
type: docs
weight: 3920
url: /ru/net/aspose.cells/jsonloadoptions/
---
## JsonLoadOptions class

Представляет параметры загрузки файлов json

```csharp
public class JsonLoadOptions : LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [JsonLoadOptions](jsonloadoptions)() | Создает опции загрузки файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Указывает, выполняется ли автоматическая фильтрация данных при загрузке файлов. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Получает и устанавливает параметры автоматической установки |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Проверить правильность данных в файле шаблона. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками. Например, excel не позволяет вводить строковое значение длиннее 32 КБ. имеет значение true, вы получите исключение. Если это свойство имеет значение false, мы примем введенное вами строковое значение в качестве значения ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако, если вы установили такое значение, которое недопустимо для формата файла Excel, вам не следует сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Получает или задает информацию о культуре системы на момент загрузки файла. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Получает и устанавливает отдельные конфигурации шрифтов. Работает только для[`Workbook`](../workbook) который использует это[`LoadOptions`](../loadoptions) для загрузки.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Игнорировать данные, которые не печатаются, при прямой печати файла |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Получает и устанавливает монитор прерываний. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Сохранять ли непроанализированные данные в памяти для книги, когда она загружается из файла шаблона. Значение по умолчанию — true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в которой сохранен файл. |
| [LayoutOptions](../../aspose.cells/jsonloadoptions/layoutoptions) { get; set; } | Варианты импорта json. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Обработчик данных для обработки данных ячеек при чтении файла шаблона. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Фильтр для обозначения способа загрузки данных. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Получает формат загрузки. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Получает или задает параметры использования памяти. |
| [MultipleWorksheets](../../aspose.cells/jsonloadoptions/multipleworksheets) { get; set; } | Указывает, импортируется ли каждый атрибут объекта JsonObject как один рабочий лист, когда все дочерние узлы являются узлами массива. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Указывает, выполняется ли разбор формулы при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Указывает, анализируются ли сводные кэшированные записи при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Получает и устанавливает пароль книги. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Получает или задает региональные параметры системы на основе CountryCode на момент загрузки файла. |
| [StartCell](../../aspose.cells/jsonloadoptions/startcell) { get; set; } | Получает и устанавливает начальную ячейку. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Устанавливает размер бумаги для печати по умолчанию из настроек принтера по умолчанию. |

### Смотрите также

* class [LoadOptions](../loadoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
