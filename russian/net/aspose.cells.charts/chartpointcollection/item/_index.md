---
title: "ChartPointCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPointCollection property. Получает элемент ChartPoint по указанному индексу в серии"
type: docs
url: /ru/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Получает элемент [`ChartPoint`](../../chartpoint/) по указанному индексу в серии.

```csharp
public ChartPoint this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс точки диаграммы в серии. |

### Возвращаемое значение

Объект ChartPoint.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к конкретной точке диаграммы с помощью свойства Item
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Изменить шаблон заливки точки
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Сохраните книгу
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


