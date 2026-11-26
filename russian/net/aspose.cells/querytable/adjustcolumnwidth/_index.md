---
title: "QueryTable.AdjustColumnWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTable. Возвращает или задает AdjustColumnWidth объекта"
type: docs
url: /ru/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Возвращает или задает AdjustColumnWidth объекта.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные с разными ширинами столбцов
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Установите ширины столбцов вручную
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Создайте таблицу запросов (симулировано, так как реальное создание требует внешнего источника данных)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Отобразите текущее значение AdjustColumnWidth
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Установите AdjustColumnWidth в true и продемонстрируйте эффект
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Смоделируйте обновление таблицы запросов (обычно регулировало бы ширины столбцов)
            // В реальном сценарии это происходит, когда таблица запросов обновляет свои данные
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Установите AdjustColumnWidth в false и продемонстрируйте эффект
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Смоделируйте повторное обновление (теперь будет сохранять исходные ширины столбцов)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Сохраните книгу
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


