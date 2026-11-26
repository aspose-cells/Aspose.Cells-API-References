---
title: "Класс DbfSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Saving.DbfSaveOptions. Представляет параметры сохранения файла dbf"
type: docs
url: /ru/net/aspose.cells.saving/dbfsaveoptions/
---
## DbfSaveOptions class

Представляет параметры сохранения файла dbf

```csharp
public class DbfSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DbfSaveOptions](dbfsaveoptions/)() | Параметры сохранения файла .dbf. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportAsString](../../aspose.cells.saving/dbfsaveoptions/exportasstring/) { get; set; } | Указывает, экспортировать ли как строковое значение |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, следует ли сортировать определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, следует ли обновлять настройки SmartArt. Значение по умолчанию — false.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, следует ли проверять объединённые ячейки перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassDbfSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте экземпляр DbfSaveOptions
            DbfSaveOptions saveOptions = new DbfSaveOptions();
            
            // Установите свойство ExportAsString
            saveOptions.ExportAsString = true;

            // Сохраните книгу с параметрами сохранения DBF
            workbook.Save("output.dbf", saveOptions);

            Console.WriteLine("Workbook saved as DBF with ExportAsString set to true.");
        }
    }
}
```

### См. также

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


