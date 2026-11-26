---
title: "Chart.SizeWithWindow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Истина, если Microsoft Excel изменяет размер диаграммы, чтобы соответствовать размеру окна листа диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

Истина, если Microsoft Excel изменяет размер диаграммы, чтобы он соответствовал размеру окна листа диаграммы.

```csharp
public bool SizeWithWindow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Продемонстрировать свойство SizeWithWindow
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // Включить SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Сохраните книгу
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


