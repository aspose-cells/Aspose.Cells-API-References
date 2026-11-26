---
title: "SparklineCollection.Remove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SparklineCollection. Удаляет спарклайн"
type: docs
url: /ru/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Удаляет спарклайн

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| o | Object |  |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод RemoveSparkline(). Этот метод будет удалён через 6 месяцев, начиная с декабря 2025 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Вставить примерные данные в рабочий лист
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Определить CellArea, где будут добавлены спарклайны
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Добавить новую SparklineGroup в рабочий лист
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Добавить спарклайны в SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Установить различные свойства для SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Установить цвета для высоких и низких точек
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Установить цвет серии и толщину линии
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Получить первый спарклайн для удаления
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Вызвать метод Remove с объектом спарклайна
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Сохраните книгу
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


