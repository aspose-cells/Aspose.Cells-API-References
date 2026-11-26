---
title: "Legend.GetLegendLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Legend. Получает метки элементов легенды после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Получает подписи записей легенды после вызова метода Chart.Calculate().

```csharp
public string[] GetLegendLabels()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
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
            
            // Вычислить диаграмму
            chart.Calculate();
            
            // Получить метки легенды
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Отобразить метки легенды
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### См. также

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


