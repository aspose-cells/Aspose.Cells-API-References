---
title: "Area.FillFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Представляет объект FillFormat, содержащий свойства форматирования заливки для указанной диаграммы или фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Представляет объект `FillFormat`, содержащий свойства форматирования заливки для указанной диаграммы или фигуры.

```csharp
public FillFormat FillFormat { get; }
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
    public class AreaPropertyFillFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите третью точку первой серии
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Задайте свойства формата заливки
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Сохраните книгу
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


