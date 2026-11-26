---
title: "Range.ExportDataTableAsString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Экспортирует данные из этого диапазона в объект DataTable"
type: docs
url: /ru/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Экспортирует данные из этого диапазона в объект DataTable.

```csharp
public DataTable ExportDataTableAsString()
```

### Возвращаемое значение

Экспортированный объект DataTable.

### Примечания

Все данные в коллекции [`Cells`](../../cells/) преобразуются в строки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Получить диапазон, содержащий данные
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Вызвать метод ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // Отобразить экспортированные данные
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Сохраните книгу
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


