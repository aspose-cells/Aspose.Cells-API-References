---
title: "ChartTextFrame.IsAutoText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Указывает, что текст генерируется автоматически"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/isautotext/
---
## ChartTextFrame.IsAutoText property

Указывает, что текст сгенерирован автоматически.

```csharp
public virtual bool IsAutoText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutoTextDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установите данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настроить заголовок диаграммы
            Aspose.Cells.Charts.ChartTextFrame title = chart.Title;
            title.Text = "Custom Chart Title";
            
            // Продемонстрировать свойство IsAutoText
            title.IsAutoText = false; // Disable auto-generated text
            
            // Сохраните книгу
            workbook.Save("ChartTextFrame_IsAutoText_Demo.xlsx");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


