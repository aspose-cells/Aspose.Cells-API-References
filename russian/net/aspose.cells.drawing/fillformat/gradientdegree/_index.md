---
title: "FillFormat.GradientDegree"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает степень градиента для указанного заполнения. Применяется только для Excel 2007"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Возвращает степень градиента для указанного заполнения. Применяется только для Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Примечания

Может принимать только значение от 0.0 (тёмный) до 1.0 (светлый).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установите градиентное заполнение для первой серии
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Отобразите степень градиента
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Сохраните книгу
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


