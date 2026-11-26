---
title: "Перечисление PlacementType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.PlacementType. Представляет способ, которым объект рисунка прикреплен к ячейкам под ним"
type: docs
url: /ru/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Представляет способ, которым объект рисунка прикреплен к расположенным ниже ячейкам.

```csharp
public enum PlacementType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| FreeFloating | `0` | Не перемещать и не изменять размер вместе с ячейками. |
| Move | `1` | Перемещать, но не изменять размер вместе с ячейками. |
| MoveAndSize | `2` | Перемещать и изменять размер вместе с ячейками. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Установите тип размещения диаграммы
            chart.Placement = PlacementType.MoveAndSize;

            // Выведите тип размещения
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Сохраните книгу
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


