---
title: "Axis.TickLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Возвращает объект TickLabels, который представляет подписи делений для указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Возвращает объект `TickLabels`, который представляет подписи делений для указанной оси.

```csharp
public TickLabels TickLabels { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Доступ к меткам делений оси категорий
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            axis.TickLabels.Font.IsBold = true;
            axis.TickLabels.Font.Color = System.Drawing.Color.Red;
            axis.TickLabels.RotationAngle = 45;
            
            // Сохраните книгу
            workbook.Save("AxisPropertyTickLabelsDemo_out.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


