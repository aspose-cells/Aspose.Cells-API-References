---
title: "ICellsDataTable.Columns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ICellsDataTable. Возвращает имена столбцов"
type: docs
url: /ru/net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Получает имя столбцов.

```csharp
public string[] Columns { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Stock");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["C2"].PutValue(15);

            try
            {
                // Экспортировать диапазон данных в ICellsDataTable
                ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 2, 3);

                // Отобразить имена столбцов
                Console.WriteLine("Column names in the data table:");
                foreach (string column in dataTable.Columns)
                {
                    Console.WriteLine(column);
                }

                // Отобразить количество столбцов
                Console.WriteLine($"Total columns: {dataTable.Columns.Length}");

                // Сохраните книгу
                workbook.Save("ColumnsDemo.xlsx");
                Console.WriteLine("Columns property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


