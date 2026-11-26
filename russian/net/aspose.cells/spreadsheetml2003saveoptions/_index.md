---
title: "Класс SpreadsheetML2003SaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SpreadsheetML2003SaveOptions. Представляет параметры сохранения файла Excel 2003 в формате spreadml"
type: docs
url: /ru/net/aspose.cells/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions class

Представляет параметры сохранения файла Excel 2003 spreadml.

```csharp
public class SpreadsheetML2003SaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor)() | Создаёт параметры для сохранения файла Excel 2003 в формате spreadml. |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor_1)(SaveFormat) | (**Obsolete.**) Создаёт параметры для сохранения файла Excel 2003 в формате spreadml. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExportColumnIndexOfCell](../../aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/) { get; set; } | Значение по умолчанию — false, это означает, что индекс столбца будет игнорироваться, если ячейка смежна с предыдущей. |
| [IsIndentedFormatting](../../aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/) { get; set; } | Заставляет дочерние элементы быть с отступом. |
| [LimitAsXls](../../aspose.cells/spreadsheetml2003saveoptions/limitasxls/) { get; set; } | Ограничение как в xls: максимальный индекс строки — 65535, а максимальный индекс столбца — 255. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsDemo
    {
        public static void SpreadsheetML2003SaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Создать экземпляр SpreadsheetML2003SaveOptions
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

            // Установить свойства
            saveOptions.IsIndentedFormatting = true;
            saveOptions.LimitAsXls = false;
            saveOptions.ExportColumnIndexOfCell = true;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Сохраните книгу с указанными параметрами сохранения
            workbook.Save("SpreadsheetML2003Example.xml", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


