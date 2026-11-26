---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartCalculateOptions. Определяет, обновлять ли все точки данных при выполнении расчёта диаграммы. По умолчанию False. Если вы хотите получить значение каждой точки данных в диаграмме, установите его в true. Если этот параметр установлен в True, новые точки данных могут быть созданы при расчёте диаграммы. Это может увеличить размер файла Excel."
type: docs
url: /ru/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Обновлять ли все точки данных при выполнении расчёта диаграммы. По умолчанию: False. Если вы хотите получить значение каждой отдельной точки данных в диаграмме, установите значение true. Если этот параметр установлен в True, новые точки данных могут быть созданы при расчёте диаграммы. Это может увеличить размер файла Excel.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Включить подписи данных
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Вычислить диаграмму с опцией UpdateAllPoints
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Вывести некоторые значения меток данных, чтобы продемонстрировать результат
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### См. также

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


