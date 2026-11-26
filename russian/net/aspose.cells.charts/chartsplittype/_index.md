---
title: "Перечисление ChartSplitType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.ChartSplitType. Представляет способ разделения двух секций либо круговой диаграммы с вложенным кругом, либо столбчатой диаграммы с вложенным кругом"
type: docs
url: /ru/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Определяет способ разбиения двух секций в диаграмме «пирог внутри пирога» или «бар внутри пирога».

```csharp
public enum ChartSplitType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Position | `0` | Представляет точки данных. Точки данных будут разделены между кругом и второй диаграммой, помещая последнюю позицию разделения точек данных во второй диаграмме. |
| Value | `1` | Представляет, что точки данных будут разделены между кругом и второй диаграммой, помещая точки данных со значением меньше позиции разделения во вторую диаграмму. |
| PercentValue | `2` | Представляет точки данных, которые будут разделены между кругом и второй диаграммой, помещая точки с процентом меньше указанного процента позиции разделения во вторую диаграмму. |
| Custom | `3` | Представляет точки данных, которые будут разделены между кругом и второй диаграммой согласно пользовательским значениям разделения. |
| Auto | `4` | Представляет точки данных, которые будут разделены с использованием механизма по умолчанию для этого типа диаграммы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте примерные данные для диаграммы
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Добавить круговую диаграмму
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Установить диапазон данных диаграммы
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Продемонстрировать различные значения ChartSplitType
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Перейти к другому типу разбиения
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Сохраните книгу
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


