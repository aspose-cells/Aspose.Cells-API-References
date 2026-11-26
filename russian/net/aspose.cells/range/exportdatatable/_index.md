---
title: "Range.ExportDataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Экспортирует данные из этого диапазона в объект DataTable"
type: docs
url: /ru/net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Экспортирует данные из этого диапазона в объект DataTable.

```csharp
public DataTable ExportDataTable()
```

### Возвращаемое значение

Экспортированный объект DataTable.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные в листе
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(450.75);

            // Создайте диапазон, содержащий данные
            Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Экспортируйте диапазон в DataTable
                DataTable dataTable = dataRange.ExportDataTable();

                Console.WriteLine("Data exported successfully to DataTable");
                Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");

                // Отобразить экспортированные данные
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}: {row[1]}");
                }

                // Измените DataTable и при необходимости импортируйте обратно
                dataTable.Rows[0]["Price"] = 1300.00;
                Console.WriteLine("\nModified first product price in DataTable to 1300.00");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting data: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("RangeMethodExportDataTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Экспортирует данные из этого диапазона в объект DataTable.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | ExportTableOptions | Параметры экспорта диапазона в DataTable. |

### Возвращаемое значение

Экспортированный объект DataTable.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class RangeMethodExportDataTableWithExportTableOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте примерные данные в листе
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Назовите диапазон, содержащий наши данные
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
            namedRange.Name = "Names";

            // Экспортируйте именованный диапазон в DataTable с параметрами
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            DataTable dataTable = namedRange.ExportDataTable(options);

            // Отобразите результаты
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### См. также

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


