---
title: "Класс TxtLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.TxtLoadOptions. Представляет параметры загрузки текстового файла"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Представляет параметры загрузки текстового файла.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Создаёт параметры для загрузки текстового файла. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Создаёт параметры для загрузки текстового файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Получает и задаёт параметры авто‑подгонки (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Проверяет, являются ли данные действительными в шаблонном файле. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, будет выброшено исключение. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата Excel, впоследствии не следует сохранять книгу в формате Excel. Иначе может возникнуть непредвиденная ошибка в сгенерированном файле Excel. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. Значение по умолчанию — true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Получает параметры стиля по умолчанию для инициализации стилей книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Получает и задает кодировку по умолчанию. Применяется только для файлов csv. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Определяет, расширять ли данные на следующий лист, когда строки или столбцы данных превышают предел. По умолчанию false. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Получает и задаёт отдельные конфигурации шрифтов. Работает только для [`Workbook`](../workbook/), который использует эти [`LoadOptions`](../loadoptions/) при загрузке. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Указывает, является ли текст формулой, если он начинается с "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Определяет, есть ли текстовый квалификатор для значения ячейки. По умолчанию true. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | Количество столбцов заголовка, которые следует повторять для расширенных листов. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | Количество строк заголовка, которые следует повторять для расширенных листов. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Указывает, следует ли игнорировать бесполезные фигуры. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Получает и задаёт монитор прерываний. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | True означает, что файл содержит несколько кодировок. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Указывает, не разбирать ли строковое значение, если его длина равна 15. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Получает или задаёт язык пользовательского интерфейса версии Workbook на основе CountryCode, в котором был сохранён файл. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Фильтр, определяющий, как загружать данные. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Получает формат загрузки. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | Максимальное количество столбцов, импортируемых в один лист. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | Максимальное количество строк, импортируемых в один лист. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задаёт режим памяти для загруженной книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, выполнять ли разбор формул при чтении файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, выполнять ли разбор кэшированных записей сводных таблиц при загрузке файла. Значение по умолчанию — false. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задаёт пароль книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Получает и задаёт предпочтительные парсеры значений для загрузки текстового файла. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и разрывы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Получает и задаёт символьный разделитель текстового файла. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Получает и задаёт строковое значение в качестве разделителя. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Устанавливает имя шрифта по умолчанию (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Устанавливает размер шрифта по умолчанию. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Определяет, следует ли рассматривать последовательные разделители как один. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Указывает, следует ли считать начальный одинарный апостроф частью значения ячейки. По умолчанию true. Если false, начальный одинарный апостроф будет удалён из соответствующего значения ячейки, и для ячейки будет установлен [`QuotePrefix`](../style/quoteprefix/) как true. |
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
    using System.Text;

    public class TxtLoadOptionsDemo
    {
        public static void TxtLoadOptionsExample()
        {
            // Создайте экземпляр TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                SeparatorString = ",",
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = '\"',
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = "password",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Загрузите CSV‑файл с указанными параметрами
            Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("TxtLoadOptionsExample.xlsx");

            return;
        }
    }

    // Фиктивные реализации для ссылочных классов/интерфейсов
    public class InterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested => false;
    }

    public class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine(warningInfo.Description);
        }
    }

    public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet) => true;
        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### См. также

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


