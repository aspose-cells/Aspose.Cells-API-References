---
title: "ChartFrame.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Возвращает объект Font указанного объекта ChartFrame"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Возвращает объект `Font` указанного объекта ChartFrame.

```csharp
public virtual Font Font { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyFontDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить заголовок диаграммы и настроить свойства шрифта
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            chart.Title.Font.Color = System.Drawing.Color.Blue;
            chart.Title.Font.CapsType = TextCapsType.None;
            chart.Title.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("ChartFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


