---
title: "TickLabels.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Возвращает объект Font, который представляет шрифт указанного объекта TickLabels"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Возвращает объект `Font`, который представляет шрифт указанного объекта TickLabels.

```csharp
public Font Font { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A1";
            
            // Получить шрифт меток делений
            Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
            Font font = tickLabels.Font;
            
            // Установите свойства шрифта
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Сохраните книгу
            workbook.Save("TickLabelsFontDemo.xlsx");
            
            Console.WriteLine("TickLabels font properties set successfully.");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


