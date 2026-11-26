---
title: "LegendEntryCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LegendEntryCollection. Получает элемент LegendEntry по указанному индексу"
type: docs
url: /ru/net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Получает элемент [`LegendEntry`](../../legendentry/) по указанному индексу.

```csharp
public LegendEntry this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Category 2");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Получите доступ к элементам легенды
            LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Продемонстрировать использование свойства Item
            for (int i = 0; i < legendEntries.Count; i++)
            {
                LegendEntry entry = legendEntries[i];
                Console.WriteLine($"Legend Entry {i}:");
                Console.WriteLine($"- Font: {entry.Font.Name}");
                Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
            }

            // Изменить первую запись легенды
            if (legendEntries.Count > 0)
            {
                legendEntries[0].Font.Name = "Arial";
                legendEntries[0].Font.Size = 12;
                legendEntries[0].AutoScaleFont = false;
            }
        }
    }
}
```

### См. также

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


