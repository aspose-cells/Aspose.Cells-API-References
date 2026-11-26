---
title: "Класс NumbersLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Numbers.NumbersLoadOptions class. Представляет параметры загрузки файлов Apple Numbers"
type: docs
url: /ru/net/aspose.cells.numbers/numbersloadoptions/
---
## NumbersLoadOptions class

Представляет параметры загрузки файлов Apple Numbers.

```csharp
public class NumbersLoadOptions : LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [NumbersLoadOptions](numbersloadoptions/)() | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Указывает, будет ли автоматически фильтроваться данные при загрузке файлов.(Наследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Получает и задает параметры автоподгонки(Наследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Проверьте, являются ли данные в шаблонном файле действительными.(Наследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Проверять ограничения файла Excel при изменении пользователем связанных с ячейками объектов. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, будет выброшено исключение. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять книгу в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel.(Наследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Получает или задает региональные настройки, используемые для Workbook, который будет загружен.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Получает настройки стиля по умолчанию для инициализации стилей workbook(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Получает и задает отдельные конфигурации шрифтов. Работает только для [`Workbook`](../../aspose.cells/workbook/), который использует эти [`LoadOptions`](../../aspose.cells/loadoptions/) для загрузки.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Указывает, следует ли игнорировать бесполезные фигуры.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Получает и задает монитор прерываний.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Нужно ли сохранять неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Получает или задает язык пользовательского интерфейса версии Workbook, основанный на CountryCode, в котором файл был сохранён.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Обработчик данных для обработки данных ячеек при чтении шаблонного файла.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Фильтр, указывающий, как загружать данные.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Получает формат загрузки.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadTableType](../../aspose.cells.numbers/numbersloadoptions/loadtabletype/) { get; set; } | Получает и задает тип загрузки нескольких таблиц в одном листе. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задает режим памяти для загруженной workbook.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, следует ли разбирать формулу при чтении файла.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задает пароль workbook.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и переносы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreserveTableName](../../aspose.cells.numbers/numbersloadoptions/preservetablename/) { get; set; } | Указывает, следует ли сохранять имена таблиц при импорте из Numbers. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Получает или задает региональные настройки, используемые для Workbook, который будет загружен.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Задает имя стандартного шрифта по умолчанию(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Задает размер стандартного шрифта по умолчанию.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Задает размер бумаги по умолчанию для печати из настроек принтера по умолчанию.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;
    using System.Globalization;

    public class NumbersLoadOptionsDemo
    {
        public static void NumbersLoadOptionsExample()
        {
            // Создать экземпляр NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Установка свойств
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                Password = "password123",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = false,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new CustomLightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new CustomWarningCallback(),
                AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true },
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = false
            };

            // Загрузить файл Numbers с указанными параметрами загрузки
            Workbook workbook = new Workbook("NumbersLoadOptionsExample_original.numbers", loadOptions);

            // Сохранить книгу в формате XLSX
            workbook.Save("NumbersLoadOptionsExample.xlsx");
        }
    }

    // Пользовательская реализация LightCellsDataHandler
    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool ProcessCell(Cell cell)
        {
            return true;
        }

        public bool ProcessRow(Row row)
        {
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            return true;
        }

        public bool StartRow(int rowIndex)
        {
            return true;
        }

        public bool StartSheet(Worksheet sheet)
        {
            return true;
        }
    }

    // Пользовательская реализация IWarningCallback
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }
}
```

### См. также

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


