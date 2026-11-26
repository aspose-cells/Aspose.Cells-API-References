---
title: "Класс SqlScriptSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Saving.SqlScriptSaveOptions. Представляет параметры сохранения SQL"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions class

Представляет параметры сохранения sql.

```csharp
public class SqlScriptSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SqlScriptSaveOptions](sqlscriptsaveoptions/)() | Создаёт параметры для сохранения файла SQL. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AddBlankLineBetweenRows](../../aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/) { get; set; } | Вставьте пустую строку между каждым набором данных. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Папка для временных файлов, которые могут использоваться как кэш данных (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckAllDataForColumnType](../../aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/) { get; set; } | Проверьте все данные, чтобы определить тип данных столбцов. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения Excel‑файла, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. При вводе значения длиннее 32 КБ оно будет усечено (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckIfTableExists](../../aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/) { get; set; } | Проверьте, существует ли имя таблицы перед созданием |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Очищать книгу после сохранения файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ColumnTypeMap](../../aspose.cells.saving/sqlscriptsaveoptions/columntypemap/) { get; set; } | Получает и задаёт отображение типов столбцов для разных баз данных. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла (наследуется от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateTable](../../aspose.cells.saving/sqlscriptsaveoptions/createtable/) { get; set; } | Указывает, экспортировать ли SQL создания таблицы. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Указывает, следует ли шифровать свойства документа при сохранении в файл .xls. Значение по умолчанию — true.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportArea](../../aspose.cells.saving/sqlscriptsaveoptions/exportarea/) { get; set; } | Получает или задает диапазон экспорта. |
| [ExportAsString](../../aspose.cells.saving/sqlscriptsaveoptions/exportasstring/) { get; set; } | Указывает, экспортировать ли все данные как строковое значение. |
| [HasHeaderRow](../../aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/) { get; set; } | Указывает, содержит ли диапазон строку заголовка. |
| [IdName](../../aspose.cells.saving/sqlscriptsaveoptions/idname/) { get; set; } | Получает и задаёт имя столбца идентификатора. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Указывает, объединять ли области условного форматирования и проверки перед сохранением файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [OperatorType](../../aspose.cells.saving/sqlscriptsaveoptions/operatortype/) { get; set; } | Получает и задаёт тип оператора SQL. |
| [PrimaryKey](../../aspose.cells.saving/sqlscriptsaveoptions/primarykey/) { get; set; } | Представляет, какой столбец является первичным ключом таблицы данных. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Указывает, кэшировать ли последние данные диаграммы.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Получает формат сохраняемого файла.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [Separator](../../aspose.cells.saving/sqlscriptsaveoptions/separator/) { get; set; } | Получает и задаёт символьный разделитель скрипта SQL. |
| [SheetIndexes](../../aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/) { get; set; } | Представляет индексы экспортируемых листов. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Указывает, следует ли сортировать внешние определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Указывает, следует ли сортировать определённые имена перед сохранением файла.(Унаследовано от [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [StartId](../../aspose.cells.saving/sqlscriptsaveoptions/startid/) { get; set; } | Получает и задаёт начальный идентификатор. |
| [TableName](../../aspose.cells.saving/sqlscriptsaveoptions/tablename/) { get; set; } | Получает и задаёт имя таблицы. |
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

    public class SqlScriptSaveOptionsDemo
    {
        public static void SqlScriptSaveOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Создайте экземпляр SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "MyTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Сохранить книгу как SQL-скрипт
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
    }
}
```

### См. также

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


