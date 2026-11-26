---
title: "FillFormat.Pattern"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Представляет шаблон отображения области"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Представляет шаблон отображения области.

```csharp
public FillPattern Pattern { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A1:A3", true);

            // Получить доступ к первой серии и её первой точке
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Установить шаблон заполнения для области точки
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Сохраните книгу
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


