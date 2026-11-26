---
title: "Класс Trendline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Trendline. Представляет линию тренда на диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/trendline/
---
## Trendline class

Представляет линию тренда на диаграмме.

```csharp
public class Trendline : Line
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward/) { get; set; } | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое линия тренда расширяется назад. Количество периодов должно быть больше или равно нулю. Если тип диаграммы — столбчатая, количество периодов должно быть от 0 до 0,5. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Указывает длину наконечника стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Указывает наконечник стрелки для начала линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Указывает конечные заглушки.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Представляет цвет линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Указывает составной тип линии(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Указывает тип пунктирной линии(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels/) { get; } | Представляет объект DataLabels для указанного ряда. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation/) { get; set; } | Отображает, отображается ли уравнение линии тренда на диаграмме (в той же подписи данных, что и значение R‑квадрата). Установка этого свойства в True автоматически включает подписи данных. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared/) { get; set; } | Отображает, отображается ли значение R‑квадрата линии тренда на диаграмме (в той же подписи данных, что и уравнение). Установка этого свойства в True автоматически включает подписи данных. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Указывает длину наконечника стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Указывает ширину наконечника стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Указывает наконечник стрелки для конца линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Получает или задает тип формата.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Forward](../../aspose.cells.charts/trendline/forward/) { get; set; } | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое линия тренда расширяется вперёд. Количество периодов должно быть больше или равно нулю. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Представляет градиентную заливку.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Intercept](../../aspose.cells.charts/trendline/intercept/) { get; set; } | Возвращает или задает точку, где линия тренда пересекает ось значений. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Указывает, автоматически ли назначен этот стиль линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Указывает, автоматически ли назначен цвет линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto/) { get; set; } | Возвращает, определяет ли Microsoft Excel автоматически название линии тренда. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Отображает, видима ли линия.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Указывает соединительные заглушки.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry/) { get; } | Получает запись легенды, соответствующую этой линии тренда |
| [Name](../../aspose.cells.charts/trendline/name/) { get; set; } | Возвращает название линии тренда. |
| [Order](../../aspose.cells.charts/trendline/order/) { get; set; } | Возвращает или задает порядок линии тренда (целое число больше 1), когда тип линии тренда — Полиномиальный. Порядок должен быть от 2 до 6. |
| [Period](../../aspose.cells.charts/trendline/period/) { get; set; } | Возвращает или задает период для линии тренда скользящего среднего. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Отображает стиль линии.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Получает и задает цвет темы.(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Возвращает или задает степень прозрачности линии как значение от 0.0 (непрозрачный) до 1.0 (прозрачный).(Наследовано от [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/trendline/type/) { get; } | Возвращает тип линии тренда. |
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
    using System.Drawing;

    public class TrendlineDemo
    {
        public static void TrendlineExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Добавление нового листа к объекту Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Добавление образцовых значений в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];
            // Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "B4"
            chart.NSeries.Add("A1:B4", true);
            // Установка источника данных для категориальных данных NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Добавление линейной линии тренда
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            // Установка пользовательского названия линии тренда
            trendline.Name = "Linear";
            // Отображение уравнения на диаграмме
            trendline.DisplayEquation = true;
            // Отображение значения R-квадрат на диаграмме
            trendline.DisplayRSquared = true;

            // Настройка дополнительных свойств
            trendline.IsNameAuto = false;
            trendline.Order = 2;
            trendline.Period = 3;
            trendline.Forward = 1.5;
            trendline.Backward = 0.5;
            trendline.Intercept = 0.0;
            trendline.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
            trendline.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.Dash;
            trendline.CapType = Aspose.Cells.Drawing.LineCapType.Round;
            trendline.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
            trendline.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
            trendline.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
            trendline.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
            trendline.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
            trendline.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
            trendline.Color = Color.Red;
            trendline.Transparency = 0.5;
            trendline.Style = Aspose.Cells.Drawing.LineType.DashDot;
            trendline.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
            trendline.WeightPt = 2.0;
            trendline.WeightPx = 3.0;
            trendline.FormattingType = Aspose.Cells.Charts.ChartLineFormattingType.Gradient;
            trendline.IsVisible = true;
            trendline.IsAuto = false;

            // Сохранение файла Excel
            workbook.Save("TrendlineExample.xlsx");
        }
    }
}
```

### См. также

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


