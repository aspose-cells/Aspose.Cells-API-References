---
title: "Axis.DisplayUnitLabel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет метку единицы на оси в указанной диаграмме. Метки единиц полезны при построении графиков больших значений, например в миллионах или миллиардах"
type: docs
url: /ru/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Представляет метку единицы на оси в указанной диаграмме. Метки единиц полезны при построении графиков больших значений — например, в миллионах или миллиардах.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A1:A4", true);
            
            // Настроить единицу отображения и метку
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Вывести текст метки единицы отображения
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Сохраните книгу
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


