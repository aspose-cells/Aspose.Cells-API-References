---
title: "Cells.MaxDataColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Максимальный индекс столбца ячейки, содержащей данные"
type: docs
url: /ru/net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Максимальный индекс столбца ячейки, содержащей данные.

```csharp
public int MaxDataColumn { get; }
```

### Примечания

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Получить максимальный индекс столбца с данными (нумерация с нуля)
            int maxColumn = worksheet.Cells.MaxDataColumn;
            Console.WriteLine("Max Data Column: " + maxColumn);

            // Экспортировать данные, используя MaxDataColumn
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 
                worksheet.Cells.MaxDataRow + 1, 
                worksheet.Cells.MaxDataColumn + 1);

            // Отобразить экспортированные данные
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                for (int i = 0; i <= maxColumn; i++)
                {
                    Console.Write(row[i] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


