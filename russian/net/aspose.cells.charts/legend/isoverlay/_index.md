---
title: "Legend.IsOverLay"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Legend. Возвращает или задает, отображать ли легенду без наложения на диаграмму"
type: docs
url: /ru/net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

Получает или задает, отображать ли легенду без перекрытия диаграммы.

```csharp
public bool IsOverLay { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyIsOverLayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Установить наложение легенды
            chart.Legend.IsOverLay = true;
            
            // Сохраните книгу
            workbook.Save("LegendOverlayDemo.xlsx");
            
            Console.WriteLine("Chart with overlay legend created successfully.");
        }
    }
}
```

### См. также

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


