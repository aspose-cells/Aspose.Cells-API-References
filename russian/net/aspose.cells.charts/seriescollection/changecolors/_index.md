---
title: "SeriesCollection.ChangeColors"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SeriesCollection. Установить монохромную палитру для серий диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Установить монохромную палитру для серий диаграммы.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ChartColorPaletteType | Монохромный тип. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Заполните диаграмму данными
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Добавить столбчатую диаграмму
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Установите диапазон данных для серии
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите коллекцию серий
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Измените цветовую палитру всех серий в коллекции.
                // Используйте числовое приведение к допустимому значению перечисления (например, 0), чтобы избежать зависимых имён членов перечисления.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Сохраните книгу, чтобы проверить результат.
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### См. также

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


