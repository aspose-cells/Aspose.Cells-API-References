---
title: "ChartTextFrame.IsAutomaticRotation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Указывает, автоматически ли вращается текст диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/isautomaticrotation/
---
## ChartTextFrame.IsAutomaticRotation property

Указывает, автоматически ли вращается текст диаграммы.

```csharp
public bool IsAutomaticRotation { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutomaticRotationDemo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к заголовку оси значений и продемонстрировать IsAutomaticRotation
            chart.ValueAxis.Title.Text = "Values";
            bool isAutoRotate = chart.ValueAxis.Title.IsAutomaticRotation;
            Console.WriteLine($"IsAutomaticRotation: {isAutoRotate}");

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


