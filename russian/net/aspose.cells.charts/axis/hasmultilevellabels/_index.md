---
title: "Axis.HasMultiLevelLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Указывает, должны ли метки отображаться многоуровнево"
type: docs
url: /ru/net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

Указывает, должны ли метки отображаться многоуровнево.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### Примечания

Действительно только для категориальной оси.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyHasMultiLevelLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример данных с многоуровневыми категориями
            worksheet.Cells["A1"].PutValue("Main Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sub Category");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Value");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(8);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите диапазон данных диаграммы, включая многоуровневые категории
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "A1:B3";
            
            // Проверьте и отобразите свойство HasMultiLevelLabels
            Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
            
            // Сохраните книгу
            workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


