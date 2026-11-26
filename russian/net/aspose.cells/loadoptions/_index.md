---
title: "Класс LoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LoadOptions. Представляет параметры загрузки файла"
type: docs
url: /ru/net/aspose.cells/loadoptions/
---
## LoadOptions class

Представляет параметры загрузки файла.

```csharp
public class LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Создаёт параметры загрузки файла. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Создаёт параметры загрузки файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Получает и задает параметры автоподгонки |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Проверьте, действительны ли данные в шаблонном файле. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиннее 32 КБ, например через Cell.PutValue(string), если это свойство равно true, вы получите исключение. Если свойство равно false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Получает или задает региональные настройки, используемые для загружаемой Workbook. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Получает параметры стиля по умолчанию для инициализации стилей рабочей книги |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Получает и задает отдельные настройки шрифтов. Работает только с [`Workbook`](../workbook/), который использует эти `LoadOptions` для загрузки. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Указывает, следует ли игнорировать бесполезные фигуры. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Получает и задает монитор прерываний. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Получает или задает язык пользовательского интерфейса версии Workbook, основанный на CountryCode, который сохранил файл. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Фильтр, указывающий, как загружать данные. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Получает формат загрузки. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задает режим памяти для загруженной рабочей книги. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, следует ли разбирать формулу при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задает пароль рабочей книги. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и переносы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Получает или задает региональные настройки, используемые для загружаемой Workbook. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Устанавливает имя стандартного шрифта по умолчанию |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Устанавливает размер стандартного шрифта по умолчанию. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Устанавливает размер бумаги по умолчанию из настроек принтера по умолчанию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // Создайте экземпляр LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Установка свойств
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Загрузите книгу с указанными LoadOptions
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Выполняйте операции над рабочей книгой
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Сохраните книгу
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


