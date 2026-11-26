---
title: "Класс ImportTableOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ImportTableOptions. Представляет параметры импорта данных в ячейки"
type: docs
url: /ru/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Представляет параметры импорта данных в ячейки.

```csharp
public class ImportTableOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Создаёт параметры импорта по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Указывает, проверять ли объединённые ячейки. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Получает или задаёт столбцы (нумерация с нуля) для импорта из источника данных. null означает, что следует импортировать все столбцы. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Указывает, применять ли стиль представления сетки к ячейкам. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Получает или задаёт значение, указывающее, следует ли преобразовывать строковое значение в числовое или дату. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Получает или задаёт строку формата даты для ячеек с импортированными значениями даты и времени. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Значение по умолчанию для ячейки в таблице — null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Указывает, экспортировать ли заголовок как имя поля. |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Указывает, следует ли добавлять новые строки при импорте записей данных. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Указывает, следует ли импортировать имя поля. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Указывает, являются ли данные формулами. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Указывает, содержит ли значение HTML‑теги. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Получает или задаёт числовые форматы. |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Указывает, сдвигать ли первую строку вниз при вставке строк. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Получает и задаёт стили для каждого столбца таблицы. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Получает или задаёт общее количество столбцов для импорта из источника данных. -1 означает все строки заданного источника данных. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Получает или задаёт общее количество строк для импорта из источника данных. -1 означает все строки заданного источника данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать DataTable для импорта.
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Создать экземпляр ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Импортировать DataTable в рабочий лист
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Сохраните книгу
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


