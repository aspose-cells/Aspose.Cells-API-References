---
title: "TickLabels.Offset"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Возвращает и задает расстояние меток от категориальной оси. Применяется только к категориальной оси X"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Получает и задает расстояние подписей от оси категорий. Это применимо только к оси категорий (x).

```csharp
public int Offset { get; set; }
```

### Примечания

Расстояние по умолчанию составляет 100 процентов, что представляет стандартный интервал между метками оси и линией оси. Значение может быть целым процентом от 0 до 1000, относительно размера шрифта метки оси.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Доступ к оси значений
            Axis valueAxis = chart.ValueAxis;
            
            // Установить смещение TickLabels
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Сохраните книгу
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


