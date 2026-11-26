---
title: "TickLabels.NumberFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Представляет строку формата для объекта TickLabels"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Представляет строку формата для объекта TickLabels.

```csharp
public string NumberFormat { get; set; }
```

### Примечания

Строка формата такая же, как пользовательская строка формата, задаваемая ячейке. Например, "$0".

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("A2:A4", true);

            // Установите числовой формат для подписей делений оси значений
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Сохраните книгу
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


