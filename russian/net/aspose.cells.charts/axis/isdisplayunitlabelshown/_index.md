---
title: "Axis.IsDisplayUnitLabelShown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает, отображается ли метка единицы на указанной оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Представляет, отображается ли метка единицы отображения на указанной оси.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Примечания

Значение по умолчанию — True. Работает только когда [`DisplayUnit`](../displayunit/) не None.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsDisplayUnitLabelShownDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Пример данных
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Настроить видимость единицы отображения и метки
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


