---
title: "FillFormat.GradientStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает стиль градиента для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Возвращает стиль градиента для указанного заполнения.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создайте диаграмму и получите её область диаграммы
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Установите стиль градиентного заполнения
            chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
            
            // Продемонстрируйте использование свойства GradientStyle
            Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
            
            // Сохраните книгу
            workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


