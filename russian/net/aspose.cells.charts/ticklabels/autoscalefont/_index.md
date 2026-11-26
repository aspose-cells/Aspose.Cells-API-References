---
title: "TickLabels.AutoScaleFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Истина, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию — Истина"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Пример данных
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Настройте данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Настройте подписи оси с помощью AutoScaleFont
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // Сохраните книгу
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


