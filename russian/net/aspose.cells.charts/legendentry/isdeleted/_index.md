---
title: "LegendEntry.IsDeleted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LegendEntry. Получает и задает, удалена ли запись легенды"
type: docs
url: /ru/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Получает и задает, удалена ли запись легенды.

```csharp
public bool IsDeleted { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Получить первую запись легенды
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // Продемонстрировать свойство IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Удалить запись легенды
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Восстановить запись легенды
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Сохраните книгу
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### См. также

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


