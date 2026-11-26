---
title: "Класс Line"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Line. Инкапсулирует объект, представляющий формат линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/
---
## Line class

Инкапсулирует объект, представляющий формат линии.

```csharp
public class Line
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Указывает длину наконечника стрелки для начала линии. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для начала линии. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Указывает наконечник стрелки для начала линии. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Указывает конечные заглушки. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Представляет цвет линии. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Указывает составной тип линии |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Указывает тип пунктирной линии |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Указывает длину наконечника стрелки для конца линии. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для конца линии. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Указывает наконечник стрелки для конца линии. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Получает или задает тип формата. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Представляет градиентную заливку. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Указывает, автоматически ли назначен этот стиль линии. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Указывает, автоматически ли назначен цвет линии. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Представляет, видима ли линия. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Указывает соединительные концы. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Представляет стиль линии. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Получает и задает цвет темы. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Возвращает или задает степень прозрачности линии значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Получает или задает [`WeightType`](../weighttype/) линии. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Получает или задает толщину линии в пунктах. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Получает или задает толщину линии в пикселях. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cells cells = sheet.Cells;
            cells[0,1].PutValue("Income");
            cells[1,0].PutValue("Company A");
            cells[2,0].PutValue("Company B");
            cells[3,0].PutValue("Company C");
            cells[1,1].PutValue(10000);
            cells[2,1].PutValue(20000);
            cells[3,1].PutValue(30000);
            
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            chart.NSeries[0].Border.Style = LineType.Dot;
            chart.NSeries[0].Border.Color = Color.Red;
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
            chart.NSeries[0].Border.Weight = WeightType.MediumLine;
            
            workbook.Save("LineChartDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


