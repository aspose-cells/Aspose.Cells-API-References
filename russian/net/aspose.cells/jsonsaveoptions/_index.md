---
title: "Класс JsonSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.JsonSaveOptions. Представляет параметры сохранения книги в файл JSON"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/
---
## JsonSaveOptions class

Представляет параметры сохранения рабочей книги в виде JSON‑файла.

```csharp
public class JsonSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [JsonSaveOptions](jsonsaveoptions/)() | Создаёт параметры для сохранения файла JSON. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AlwaysExportAsJsonObject](../../aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/) { get; set; } | Указывает, следует ли всегда экспортировать Excel в JSON как объект, даже если в файле только один лист. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/jsonsaveoptions/exportarea/) { get; set; } | Получает или задает диапазон экспорта. |
| [ExportAsString](../../aspose.cells/jsonsaveoptions/exportasstring/) { get; set; } | Экспортирует строковое значение ячеек в JSON. |
| [ExportEmptyCells](../../aspose.cells/jsonsaveoptions/exportemptycells/) { get; set; } | Указывает, экспортировать ли пустые ячейки как null. |
| [ExportHyperlinkType](../../aspose.cells/jsonsaveoptions/exporthyperlinktype/) { get; set; } | Представляет тип экспорта гиперссылок в JSON. |
| [ExportNestedStructure](../../aspose.cells/jsonsaveoptions/exportnestedstructure/) { get; set; } | Экспортировано как иерархическая структура JSON типа «родитель‑дитя». |
| [ExportStylePool](../../aspose.cells/jsonsaveoptions/exportstylepool/) { get; set; } | Указывает, экспортировать стили совместно или индивидуально для каждой ячейки. |
| [HasHeaderRow](../../aspose.cells/jsonsaveoptions/hasheaderrow/) { get; set; } | Указывает, содержит ли диапазон строку заголовка. |
| [Indent](../../aspose.cells/jsonsaveoptions/indent/) { get; set; } | Указывает отступ. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [Schemas](../../aspose.cells/jsonsaveoptions/schemas/) { get; set; } | Исходная схема JSON каждой таблицы. |
| [SheetIndexes](../../aspose.cells/jsonsaveoptions/sheetindexes/) { get; set; } | Представляет индексы экспортируемых листов. |
| [SkipEmptyRows](../../aspose.cells/jsonsaveoptions/skipemptyrows/) { get; set; } | Указывает, пропускать ли пустые строки. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ToExcelStruct](../../aspose.cells/jsonsaveoptions/toexcelstruct/) { get; set; } | Указывает, преобразовывать ли в структуру JSON файла Excel. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonSaveOptionsDemo
    {
        public static void JsonSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте экземпляр JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = "  ",
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Сохраните книгу в файл JSON
            workbook.Save("JsonSaveOptionsExample.json", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


