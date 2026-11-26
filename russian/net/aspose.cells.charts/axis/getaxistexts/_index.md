---
title: "Axis.GetAxisTexts"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Axis. Получает подписи оси после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

Получает метки оси после вызова метода Chart.Calculate().

```csharp
public string[] GetAxisTexts()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisMethodGetAxisTextsDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(4000);
            worksheet.Cells["B4"].PutValue(-8000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Вычислить диаграмму
            chart.Calculate();
            
            // Получить подписи оси
            string[] labels = chart.ValueAxis.GetAxisTexts();
            
            // Вывести подписи
            Console.WriteLine("Value Axis Labels:");
            foreach (string label in labels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


