---
title: "Класс ErrorBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ErrorBar. Представляет полосу ошибок серии данных."
type: docs
url: /ru/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Представляет линию ошибок серии данных.

```csharp
public class ErrorBar : Line
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Представляет величину полосы ошибок. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Указывает длину наконечника стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Указывает наконечник стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Указывает конечные заглушки.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Представляет цвет линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Указывает составной тип линии(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Указывает тип пунктирной линии(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Представляет тип отображения полосы ошибок. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Указывает длину наконечника стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Указывает наконечник стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Получает или задает тип формата.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Представляет градиентную заливку.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Указывает, автоматически ли назначен этот стиль линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Указывает, автоматически ли назначен цвет линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Отображает, видима ли линия.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Указывает соединительные заглушки.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Представляет отрицательную величину ошибки, когда тип полосы ошибок установлен как Custom. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Представляет положительную величину ошибки, когда тип полосы ошибок установлен как Custom. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Указывает, следует ли форматировать полосы ошибок с верхушкой‑Т. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Отображает стиль линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Получает и задает цвет темы.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Возвращает или задает степень прозрачности линии как значение от 0.0 (непрозрачный) до 1.0 (прозрачный).(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Представляет тип величины полосы ошибок. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Получает или задает [`WeightType`](../../aspose.cells.drawing/weighttype/) линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Получает или задает толщину линии в единицах пунктов.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Получает или задает толщину линии в единицах пикселей.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDemo
    {
        public static void ErrorBarExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавить примерные данные в ячейки
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);
            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Добавить диаграмму в лист
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Добавьте NSeries (источник данных диаграммы) к диаграмме
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Настроить линии ошибок для каждой серии в диаграмме
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Дополнительные свойства для демонстрации
                series.YErrorBar.ShowMarkerTTop = true;
                series.YErrorBar.PlusValue = "=Sheet1!A1";
                series.YErrorBar.MinusValue = "=Sheet1!A2";
                series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
                series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
                series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
                series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
                series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
                series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
                series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
                series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
                series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
                series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
                series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
                series.YErrorBar.Color = System.Drawing.Color.Red;
                series.YErrorBar.Transparency = 0.5;
                series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
                series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
                series.YErrorBar.WeightPt = 2.0;
                series.YErrorBar.WeightPx = 3.0;
                series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
                series.YErrorBar.IsVisible = true;
                series.YErrorBar.IsAuto = false;
            }

            // Сохраните книгу
            workbook.Save("ErrorBarExample.xlsx");
            workbook.Save("ErrorBarExample.pdf");
        }
    }
}
```

### См. также

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


