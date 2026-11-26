---
title: "TickLabels.RotationAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Представляет угол поворота текста по часовой стрелке"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Представляет угол поворота текста по часовой стрелке.

```csharp
public int RotationAngle { get; set; }
```

### Примечания

0: Не вращено.255: Сверху вниз.-90: Вниз.90: Вверх.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Поверните подписи делений категориальной оси на 45 градусов
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Сохраните книгу
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


