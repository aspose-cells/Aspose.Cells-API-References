---
title: "SparklineGroupCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroupCollection. Получает элемент SparklineGroup по указанному индексу"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Получает элемент [`SparklineGroup`](../../sparklinegroup/) по указанному индексу.

```csharp
public SparklineGroup this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавьте примерные данные
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Определите диапазон данных и расположение для sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Добавить группу спарклайнов
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Получите доступ к группе спарклайнов, используя свойство Item
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Настройте спарклайн
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Сохраните книгу
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


