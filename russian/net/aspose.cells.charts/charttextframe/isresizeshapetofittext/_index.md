---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Получает или задает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка происходит, когда текст внутри формы масштабируется, чтобы вместить весь текст"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Получает или задает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это масштабирование текста внутри формы для размещения всего текста.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить данные серии
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Получить доступ к меткам данных
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // Продемонстрировать свойство IsResizeShapeToFitText
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Отключить автоматическое изменение размера формы для размещения текста
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Установить пользовательскую ширину, меньшую, чем обычно требуется для текста
                point.DataLabels.Width = 50;
            }

            // Сохраните книгу
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


