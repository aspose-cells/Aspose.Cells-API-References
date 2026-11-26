---
title: "Класс XlsbSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.XlsbSaveOptions. Представляет параметры для сохранения файла xlsb"
type: docs
url: /ru/net/aspose.cells/xlsbsaveoptions/
---
## XlsbSaveOptions class

Представляет параметры сохранения файла xlsb.

```csharp
public class XlsbSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XlsbSaveOptions](xlsbsaveoptions/#constructor)() | Создаёт параметры сохранения файла xlsb. |
| [XlsbSaveOptions](xlsbsaveoptions/#constructor_1)(SaveFormat) | (**Obsolete.**) Создаёт параметры сохранения файла xlsb. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/xlsbsaveoptions/compressiontype/) { get; set; } | Получает и задает тип сжатия для файла ooxml. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ExportAllColumnIndexes](../../aspose.cells/xlsbsaveoptions/exportallcolumnindexes/) { get; set; } | Указывает, экспортировать ли все индексы столбцов для ячеек. |
| [LightCellsDataProvider](../../aspose.cells/xlsbsaveoptions/lightcellsdataprovider/) { get; set; } | Поставщик данных для сохранения книги в лёгком режиме. |
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

    public class XlsbSaveOptionsDemo
    {
        public static void XlsbSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создать экземпляр XlsbSaveOptions
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6,
                ExportAllColumnIndexes = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Сохранить книгу как файл XLSB с указанными параметрами
            workbook.Save("XlsbSaveOptionsExample.xlsb", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


