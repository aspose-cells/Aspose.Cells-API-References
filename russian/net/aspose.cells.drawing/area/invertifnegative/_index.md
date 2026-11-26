---
title: "Area.InvertIfNegative"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Если свойство истинно и значение точки диаграммы отрицательное, foreground color и background color будут обменены"
type: docs
url: /ru/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Если свойство истинно и значение точки диаграммы отрицательное, цвета переднего плана и фона будут обменены.

```csharp
public bool InvertIfNegative { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные с отрицательным значением
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте серию данных и настройте свойства области
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### См. также

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


