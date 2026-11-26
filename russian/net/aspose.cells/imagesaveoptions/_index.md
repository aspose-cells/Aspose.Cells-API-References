---
title: "Класс ImageSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ImageSaveOptions. Представляет параметры сохранения изображения. Для расширенного использования, пожалуйста, используйте WorkbookRender или SheetRender"
type: docs
url: /ru/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Представляет параметры сохранения изображения. Для расширенного использования, пожалуйста, используйте [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) или [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Создаёт параметры для сохранения файла изображения. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Создаёт параметры для сохранения файла изображения. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в формате .xls. Значение по умолчанию — true. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Дополнительные параметры создания изображения. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, сортировать ли внешние определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, сортировать ли определённые имена перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Получает или задает IStreamProvider для экспорта объектов. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, обновлять ли настройки SmartArt. Значение по умолчанию — false. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, проверять ли объединённые ячейки перед сохранением файла. (Наследовано от [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задает обратный вызов предупреждения. (Унаследовано от [`SaveOptions`](../saveoptions/).) |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // Установить путь назначения
            string destPath = "output.png";

            // Создать параметры сохранения изображения
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Настроить параметры сохранения
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // Сохранить книгу с параметрами изображения
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


