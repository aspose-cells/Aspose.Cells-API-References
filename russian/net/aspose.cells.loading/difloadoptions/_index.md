---
title: "Класс DifLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Loading.DifLoadOptions. Представляет параметры загрузки файла .dif"
type: docs
url: /ru/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Представляет параметры загрузки файла .dif.

```csharp
public class DifLoadOptions : LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Параметры. |

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
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задает режим памяти для загруженной workbook.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, следует ли разбирать формулу при чтении файла.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задает пароль workbook.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и переносы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.(Унаследовано от [`LoadOptions`](../../aspose.cells/loadoptions/).) |
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
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // Создать экземпляр DifLoadOptions
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Создать workbook (используя конструктор без параметров)
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Вычислите формулы, если они есть
            workbook.CalculateFormula();

            // Сохраните книгу в формате DIF
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Теперь продемонстрируйте загрузку файла DIF с помощью DifLoadOptions
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Загрузите сохранённый файл DIF с указанными параметрами
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Получите доступ к данным загруженной книги
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Сохраните загруженные данные в XLSX для проверки
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


