---
title: "PatternFill.Pattern"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PatternFill. Получает или задает тип шаблона заливки"
type: docs
url: /ru/net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

Получает или задает тип шаблона заполнения.

```csharp
public FillPattern Pattern { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyPatternDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Установите шаблон заливки для первой серии
            chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
            chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
            
            // Сохраните книгу
            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


