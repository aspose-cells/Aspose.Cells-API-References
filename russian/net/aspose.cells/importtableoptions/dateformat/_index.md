---
title: "ImportTableOptions.DateFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает или задает строку формата даты для ячеек с импортированными значениями datetime"
type: docs
url: /ru/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Получает или задаёт строку формата даты для ячеек с импортированными значениями даты и времени.

```csharp
public string DateFormat { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте примерный DataTable с датами
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Определите диапазон импорта
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Импортировать данные с пользовательским форматом даты
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Сохранить книгу, чтобы продемонстрировать результат
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


