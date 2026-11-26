---
title: "Класс HtmlLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.HtmlLoadOptions. Представляет параметры при импорте HTML‑файла"
type: docs
url: /ru/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Представляет параметры при импорте HTML‑файла.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | Создаёт параметры загрузки файла. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | Создаёт параметры загрузки файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) Каталог, в который будут сохраняться вложенные файлы. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Указывает, следует ли автоматически подгонять столбцы и строки. Значение по умолчанию — false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Получает и задаёт параметры авто‑подгонки (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Проверяет, являются ли данные действительными в шаблонном файле. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Определяет, проверять ли ограничения файла Excel при изменении пользователем объектов, связанных с ячейками. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, будет выброшено исключение. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата Excel, впоследствии не следует сохранять книгу в формате Excel. Иначе может возникнуть непредвиденная ошибка в сгенерированном файле Excel. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. Значение по умолчанию — true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) если true, преобразовать строку в формулу, когда значение строки начинается с символа '=', значение по умолчанию — false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Получает параметры стиля по умолчанию для инициализации стилей книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Указывает, следует ли удалять лишние пробелы при переносе строк текста с использованием тега `<br>`. Значение по умолчанию — false. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Указывает, следует ли обнаруживать LaTeX‑формулы в HTML‑файле. Значение по умолчанию — false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Получает и задает кодировку по умолчанию. Применяется только для файлов csv. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Получает и задаёт отдельные конфигурации шрифтов. Работает только для [`Workbook`](../workbook/), который использует эти [`LoadOptions`](../loadoptions/) при загрузке. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Указывает, является ли текст формулой, если он начинается с "=". |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Определяет, как загружаются гиперссылки при загрузке HTML. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Указывает, следует ли игнорировать бесполезные фигуры. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Получает и задаёт монитор прерываний. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Указывает, не разбирать ли строковое значение, если его длина равна 15. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Получает или задаёт язык пользовательского интерфейса версии Workbook на основе CountryCode, в котором был сохранён файл. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Обработчик данных для обработки данных ячеек при чтении шаблонного файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Фильтр, определяющий, как загружать данные. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Получает формат загрузки. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Указывает, следует ли импортировать формулы, если исходный HTML‑файл содержит формулы |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. (Наследовано от [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Получает или задаёт режим памяти для загруженной книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Указывает, как отображаются элементы HTML &lt;p&gt; при загрузке HTML. Значение по умолчанию — Normal. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Указывает, как отображаются элементы HTML &lt;p&gt; при загрузке HTML. Значение по умолчанию — Normal. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Указывает, выполнять ли разбор формул при чтении файла. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, выполнять ли разбор кэшированных записей сводных таблиц при загрузке файла. Значение по умолчанию — false. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Получает и задаёт пароль книги. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и разрывы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Получает идентификатор программы, создавшей файл. Только для файлов MHT. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Получает или задаёт региональные настройки, используемые для загружаемой книги Workbook. (Наследовано от [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Устанавливает имя шрифта по умолчанию (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Устанавливает размер шрифта по умолчанию. (Унаследовано от [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Получает или задает StreamProviderImportHtmlFile для импорта объектов. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Указывает, поддерживается ли макет тега `<div>`, когда HTML‑файл содержит его. Значение по умолчанию — false. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Получить экземпляр HtmlTableLoadOptionCollection |
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
    using System.IO;

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // Создать экземпляр HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // Загрузить HTML‑файл в Workbook с использованием HtmlLoadOptions
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


