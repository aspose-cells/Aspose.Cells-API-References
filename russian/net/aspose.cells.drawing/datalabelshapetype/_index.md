---
title: "Перечисление DataLabelShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.DataLabelShapeType. Указывает предустановленную геометрию формы, которая будет использоваться для диаграммы"
type: docs
url: /ru/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Указывает предустановленную геометрию фигуры, которая будет использоваться для диаграммы.

```csharp
public enum DataLabelShapeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Rect | `0` | Представляет прямоугольную форму. |
| RoundRect | `1` | Представляет форму закруглённого прямоугольника. |
| Ellipse | `2` | Представляет форму эллипса. |
| RightArrowCallout | `3` | Представляет форму выноски со стрелкой вправо. |
| DownArrowCallout | `4` | Представляет форму выноски со стрелкой вниз. |
| LeftArrowCallout | `5` | Представляет форму выноски со стрелкой влево. |
| UpArrowCallout | `6` | Представляет форму выноски со стрелкой вверх. |
| WedgeRectCallout | `7` | Представляет форму выноски в виде клина прямоугольника. |
| WedgeRoundRectCallout | `8` | Представляет форму выноски в виде клина закруглённого прямоугольника. |
| WedgeEllipseCallout | `9` | Представляет форму выноски в виде клина эллипса. |
| LineCallout | `10` | Представляет форму выноски в виде линии. |
| BentLineCallout | `11` | Представляет форму выноски в виде изогнутой линии. |
| LineWithAccentBarCallout | `12` | Представляет форму выноски в виде линии с акцентирующей полосой. |
| BentLineWithAccentBarCallout | `13` | Представляет форму выноски в виде изогнутой линии с акцентирующей полосой. |
| Line | `14` | Этот тип используется только для специальной обработки файлов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
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

            // Получить доступ к первой серии на диаграмме
            Series series = chart.NSeries[0];

            // Включить подписи данных для серии.
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Сохраните книгу
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


