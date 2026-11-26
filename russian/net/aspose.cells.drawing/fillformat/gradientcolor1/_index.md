---
title: "FillFormat.GradientColor1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает градиентный цвет 1 для указанного заполнения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Возвращает градиентный цвет 1 для указанной заливки.

```csharp
public Color GradientColor1 { get; }
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
    public class FillFormatPropertyGradientColor1Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Получить формат заполнения первой серии
            FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            
            // Создать градиентное заполнение, используя правильные типы параметров
            fillFormat.SetTwoColorGradient(
                Color.Red, 
                Color.White, 
                GradientStyleType.Horizontal, 
                1); // Gradient variant must be integer (1-4)

            // Получить и отобразить градиентный цвет
            Color gradientColor1 = fillFormat.GradientColor1;
            Console.WriteLine("Gradient Color 1: " + gradientColor1);
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


