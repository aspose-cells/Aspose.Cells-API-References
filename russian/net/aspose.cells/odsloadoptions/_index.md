---
title: OdsLoadOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры загрузки файла ods.
type: docs
weight: 4330
url: /ru/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Представляет параметры загрузки файла ods.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OdsLoadOptions](odsloadoptions#constructor)() | Представляет параметры загрузки файла ods. |
| [OdsLoadOptions](odsloadoptions#constructor_1)(LoadFormat) | Представляет параметры загрузки файла ods. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink) { get; set; } | Указывает, применяется ли стиль Excel по умолчанию к гиперссылке. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Указывает, выполняется ли автоматическая фильтрация данных при загрузке файлов. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Получает и устанавливает параметры автоматической установки |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Проверить правильность данных в файле шаблона. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками. Например, Excel не позволяет вводить строковое значение длиннее 32 КБ. Когда вы вводите значение длиннее 32 КБ, например Cell.PutValue(string), если это свойство истинно, вы получите исключение. Если это свойство имеет значение false, мы примем введенное вами строковое значение в качестве значения ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако, если вы установили такое значение, которое недопустимо для формата файла Excel, вам не следует сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Получает или задает информацию о культуре системы на момент загрузки файла. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Получает настройки стиля по умолчанию для инициализации стилей книги |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Получает и устанавливает отдельные конфигурации шрифтов. Работает только для[`Workbook`](../workbook)который использует этот[`LoadOptions`](../loadoptions)для загрузки.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Игнорировать нераспечатанные данные при прямой печати файла |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Получает и устанавливает монитор прерываний. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Сохранять ли непроанализированные данные в памяти для рабочей книги, когда она загружается из файла шаблона. Значение по умолчанию верно. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в котором сохранен файл. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Обработчик данных для обработки данных ячеек при чтении файла шаблона. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Фильтр для обозначения способа загрузки данных. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Получает формат загрузки. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Получает или задает параметры использования памяти. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Указывает, выполняется ли разбор формулы при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Указывает, выполняется ли разбор сводных кэшированных записей при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Получает и устанавливает пароль книги. |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables) { get; set; } | Указывает, обновлять ли сводные таблицы при загрузке файла. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Получает или задает региональные параметры системы на основе CountryCode на момент загрузки файла. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Получает или устанавливает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Устанавливает размер бумаги для печати по умолчанию из настроек принтера по умолчанию. |

### Смотрите также

* class [LoadOptions](../loadoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
