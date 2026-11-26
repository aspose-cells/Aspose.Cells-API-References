---
title: "Класс SaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SaveOptions. Представляет все параметры сохранения"
type: docs
url: /ru/net/aspose.cells/saveoptions/
---
## SaveOptions class

Представляет все параметры сохранения

```csharp
public class SaveOptions
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Сделать книгу пустой после сохранения файла. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, следует ли объединять области условного форматирования и проверки данных перед сохранением файла. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, следует ли кэшировать последние данные диаграммы. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла. |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, следует ли сортировать определённые имена перед сохранением файла. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Указывает, следует ли обновлять настройку Smart Art. Значение по умолчанию — false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Указывает, следует ли проверять объединённые ячейки перед сохранением файла. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Получает или задаёт обратный вызов предупреждения. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSaveOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Создайте параметры сохранения — сохранить как CSV
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            
            // Создайте параметры загрузки для CSV
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Пересохраните книгу, используя параметры
            Workbook resavedWorkbook = Cells_Type_SaveOptions(workbook, saveOptions, loadOptions);

            // Сохраните результат в файл
            resavedWorkbook.Save("output.csv", SaveFormat.Csv);
        }

        public static Workbook Cells_Type_SaveOptions(Workbook wb, SaveOptions optsSave, LoadOptions optsLoad)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                wb.Save(ms, optsSave);
                ms.Position = 0;
                return new Workbook(ms, optsLoad);
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


