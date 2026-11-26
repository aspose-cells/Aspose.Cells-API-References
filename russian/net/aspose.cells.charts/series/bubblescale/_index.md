---
title: "Series.BubbleScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает или задает коэффициент масштабирования пузырей в указанной группе диаграмм. Может принимать целое значение от 0 до 300, соответствующее проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам"
type: docs
url: /ru/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Получает или задает коэффициент масштабирования пузырей в указанной группе диаграмм. Это может быть целое значение от 0 (ноль) до 300, соответствующее проценту от размера по умолчанию. Применяется только к пузырьковым диаграммам.

```csharp
public int BubbleScale { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример данных для пузырчатой диаграммы
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Добавить пузырчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию к диаграмме
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Установите масштаб пузырей, чтобы продемонстрировать свойство
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Настройте внешний вид диаграммы
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Сохраните книгу
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


