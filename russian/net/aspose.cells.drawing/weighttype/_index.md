---
title: "Перечисление WeightType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.WeightType enum. Перечисляет типы толщины для границы изображения или линии диаграммы"
type: docs
url: /ru/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Перечисляет типы толщины для границы изображения или линии диаграммы.

```csharp
public enum WeightType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| HairLine | `-1` | Представляет толщину тонкой линии. |
| MediumLine | `1` | Представляет толщину средней линии. |
| SingleLine | `0` | Представляет толщину одинарной линии. |
| WideLine | `2` | Представляет толщину широкой линии. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте диаграмму и получите её область диаграммы
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Установите тип толщины границы
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Проверьте тип толщины
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Сохраните книгу
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


