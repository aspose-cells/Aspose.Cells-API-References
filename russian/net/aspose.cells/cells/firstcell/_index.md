---
title: "Cells.FirstCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает первую ячейку в этом листе"
type: docs
url: /ru/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Получает первую ячейку в этом листе.

```csharp
public Cell FirstCell { get; }
```

### Примечания

Возвращает null, если в листе нет данных.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Получить коллекцию ячеек
            Cells cells = worksheet.Cells;
            
            // Продемонстрировать свойство FirstCell
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // Создайте диаграмму, используя FirstCell и LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Сохраните книгу
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


