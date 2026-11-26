---
title: "Класс XpsSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.XpsSaveOptions. Представляет дополнительные параметры при сохранении файла в формате Xps"
type: docs
url: /ru/net/aspose.cells/xpssaveoptions/
---
## XpsSaveOptions class

Представляет дополнительные параметры при сохранении файла в формате Xps.

```csharp
public class XpsSaveOptions : PaginatedSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XpsSaveOptions](xpssaveoptions/#constructor)() | Создаёт параметры для сохранения файла xps. |
| [XpsSaveOptions](xpssaveoptions/#constructor_1)(SaveFormat) | (**Устарело.**) Создаёт параметры для сохранения файла xps. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Если значение AllColumnsInOnePagePerSheet равно true, всё содержимое столбцов одного листа будет выводиться только на одну страницу в результате. Ширина размера бумаги в настройках pagesetup будет игнорироваться, а остальные настройки pagesetup по‑прежнему будут применяться. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf, изображении. Установите значение true, чтобы попытаться сначала использовать шрифт по умолчанию книги для отображения этих символов. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Получает или задаёт пользовательские настройки во время рендеринга. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Получает или задаёт язык редактирования по умолчанию. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Когда символы в Excel являются Unicode и в стиле ячейки не установлен правильный шрифт, они могут отображаться как блоки в pdf, изображении. Установите DefaultFont, например MingLiu или MS Gothic, чтобы отобразить эти символы. Если это свойство не задано, Aspose.Cells будет использовать системный шрифт по умолчанию для отображения этих Unicode‑символов. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Реализует этот интерфейс для получения DrawObject и Bound при рендеринге. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Настройка рендеринга метафайла Emf. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Получает или задаёт цвет линий сетки. (Наследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Получает или задает тип линий сетки.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Указывает, нужно ли скрывать ошибку при рендеринге. Ошибка может быть связана с фигурой, изображением, рендерингом диаграммы и т.д.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Если OnePagePerSheet установлен в true, всё содержимое листа будет выводиться только на одну страницу в результате. Размер бумаги в настройках страницы будет недействительным, а остальные настройки страницы сохранят действие.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Указывает, следует ли выводить пустую страницу, когда нечего печатать.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Получает или задает количество страниц для сохранения.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Получает или задает нулевой индекс первой страницы для сохранения.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Управляет/указывает прогресс процесса сохранения страниц.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Указывает, какие страницы не будут печататься.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Получает или задает специфические для Excel поведения рендеринга, которые следует применить.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки.(Унаследовано от [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsDemo
    {
        public static void XpsSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Создать XpsSaveOptions с определёнными настройками
            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = false,
                OutputBlankPageWhenNothingToPrint = false,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.Default,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.Default,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.All
            };

            // Сохранить книгу как XPS с указанными параметрами
            workbook.Save("XpsSaveOptionsExample.xps", saveOptions);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


