---
title: "Chart.Floor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает объект Floor, представляющий стены 3D‑диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Возвращает объект `Floor`, представляющий стены 3‑D диаграммы.

```csharp
public Floor Floor { get; }
```

### Примечания

Это свойство не применяется к 3-D круговым диаграммам.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyFloorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ и изменить свойства пола
            Floor floor = chart.Floor;
            floor.FillFormat.SetTwoColorGradient(System.Drawing.Color.LightBlue, System.Drawing.Color.DarkBlue, GradientStyleType.Horizontal, 2);
            floor.Border.Color = System.Drawing.Color.Black;

            // Сохраните книгу
            workbook.Save("ChartFloorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


