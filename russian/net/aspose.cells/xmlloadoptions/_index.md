---
title: "Класс XmlLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.XmlLoadOptions класс. Представляет параметры загрузки xml"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/
---
## XmlLoadOptions class

Представляет параметры загрузки xml.

```csharp
public class XmlLoadOptions : LoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XmlLoadOptions](xmlloadoptions/#constructor)() | Представляет параметры загрузки xml‑файла. |
| [XmlLoadOptions](xmlloadoptions/#constructor_1)(LoadFormat) | Представляет параметры загрузки xml‑файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Получает и задаёт параметры авто‑подгонки (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Проверяет, являются ли данные действительными в шаблонном файле. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, будет выброшено исключение. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата Excel, впоследствии не следует сохранять книгу в формате Excel. Иначе может возникнуть непредвиденная ошибка в сгенерированном файле Excel. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ContainsMultipleWorksheets](../../aspose.cells/xmlloadoptions/containsmultipleworksheets/) { get; set; } | Указывает, импортировать ли xml как несколько листов. |
| [ConvertNumericOrDate](../../aspose.cells/xmlloadoptions/convertnumericordate/) { get; set; } | Указывает, преобразовывать ли значение в xml‑файле в числовое или дату. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [DateFormat](../../aspose.cells/xmlloadoptions/dateformat/) { get; set; } | Получает и задает формат значения даты. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Получает параметры стиля по умолчанию для инициализации стилей книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Получает и задаёт отдельные конфигурации шрифтов. Работает только для [`Workbook`](../workbook/), который использует эти [`LoadOptions`](../loadoptions/) при загрузке. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IgnoreRootAttributes](../../aspose.cells/xmlloadoptions/ignorerootattributes/) { get; set; } | Указывает, следует ли игнорировать атрибуты корневого элемента. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Указывает, следует ли игнорировать бесполезные фигуры. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Получает и задаёт монитор прерываний. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IsXmlMap](../../aspose.cells/xmlloadoptions/isxmlmap/) { get; set; } | Указывает, следует ли сопоставлять XML с Excel. Значение по умолчанию — false. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Получает или задаёт язык пользовательского интерфейса версии Workbook на основе CountryCode, в котором был сохранён файл. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Фильтр, определяющий, как загружать данные. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Получает формат загрузки. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задаёт режим памяти для загруженной книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [NumberFormat](../../aspose.cells/xmlloadoptions/numberformat/) { get; set; } | Получает и задает формат числового значения. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, выполнять ли разбор формул при чтении файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, выполнять ли разбор кэшированных записей сводных таблиц при загрузке файла. Значение по умолчанию — false. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задаёт пароль книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и разрывы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Устанавливает имя шрифта по умолчанию (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Устанавливает размер шрифта по умолчанию. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [StartCell](../../aspose.cells/xmlloadoptions/startcell/) { get; set; } | Получает и задает начальную ячейку. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`LoadOptions`](../loadoptions/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Устанавливает размер бумаги по умолчанию из настроек принтера. (Унаследовано от [`LoadOptions`](../loadoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsDemo
    {
        public static void XmlLoadOptionsExample()
        {
            // Создайте экземпляр XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Установка свойств
            options.StartCell = "A1";
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = "0.00";
            options.DateFormat = "yyyy-MM-dd";
            options.IgnoreRootAttributes = false;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            options.LightCellsDataHandler = null; // Assuming no data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = null; // Assuming no individual font configs are set
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = false;

            // Загрузите XML‑файл в Workbook, используя указанные параметры
            Workbook workbook = new Workbook("XmlLoadOptionsExample_original.xml", options);
            workbook.DefaultStyle.Font.Name = "Arial";  
            workbook.DefaultStyle.Font.Size = 10;
            
            // Сохраните книгу в новый файл
            workbook.Save("XmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


