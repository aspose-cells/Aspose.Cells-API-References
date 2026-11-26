---
title: "Класс MarkdownSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.MarkdownSaveOptions. Представляет параметры сохранения для markdown"
type: docs
url: /ru/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Представляет параметры сохранения markdown.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Создаёт параметры для сохранения markdown-документа |

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Указывает, включено ли выравнивание столбцов для сгенерированных таблиц Markdown. При включении столбцы выравниваются путем заполнения содержимого ячеек указанным символом (обычно ' ' для пробелов). Установите "\\0", чтобы отключить выравнивание столбцов (по умолчанию). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Указывает, следует ли вычислять формулы перед сохранением markdown-файла. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Получает и задает кодировку по умолчанию. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Указывает, экспортировать ли гиперссылку с использованием определений ссылок вместо встроенного формата. Значение по умолчанию — false. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Указывает, сохраняются ли изображения в формате Base64 в Markdown. Значение по умолчанию — true. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Получает и задает стратегию форматирования при экспорте значения ячейки как строки. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Получите объект ImageOrPrintOptions перед экспортом |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | Поставщик данных для предоставления данных ячеек при сохранении книги в облегчённом режиме. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Получает и задает разделитель строк. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | Указывает, как объекты OfficeMath экспортируются в Markdown, значение по умолчанию — Image. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Указывает, следует ли рассматривать пустые строки в листе как разделители таблиц при экспорте в Markdown. Значение по умолчанию — false. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Получает или задает IStreamProvider для экспорта объектов. Если `null`, экспортированные объекты будут сохранены в той же директории, что и выходной файл. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Получает и задает способ установки заголовка таблицы. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Создайте экземпляр MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Сохраните книгу в виде файла Markdown
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


