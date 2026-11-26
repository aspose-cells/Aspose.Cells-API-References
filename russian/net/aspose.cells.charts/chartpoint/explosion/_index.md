---
title: "ChartPoint.Explosion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Расстояние открытого куска пирога от центра круговой диаграммы выражается в процентах от диаметра пирога"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

Расстояние открытого сектора круговой диаграммы от её центра выражается в процентах от диаметра диаграммы.

```csharp
public int Explosion { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyExplosionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую точку диаграммы и установить взрыв
            ChartPoint point = chart.NSeries[0].Points[0];
            point.Explosion = 15; // Set explosion distance (15 points)

            // Сохраните книгу
            workbook.Save("ChartPointExplosionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


