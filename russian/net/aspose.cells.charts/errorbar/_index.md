---
title: ErrorBar
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет планку погрешностей ряда данных.
type: docs
weight: 630
url: /ru/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Представляет планку погрешностей ряда данных.

```csharp
public class ErrorBar : Line
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Представляет количество ошибок bar.  Сумма должна быть больше или равна нулю. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Определяет длину стрелки для начала строки. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Определяет ширину стрелки для начала строки. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Указывает стрелку для начала строки. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Указывает конечные заглавные буквы. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | ПредставляетColor линии. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Указывает тип составной линии |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Определяет тип пунктирной линии |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Представляет тип отображения панели ошибок. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Определяет длину стрелки для конца строки. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Определяет ширину стрелки для конца строки. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Указывает конец строки со стрелкой. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Получает или задает тип формата. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Представляет градиентную заливку. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Указывает, назначается ли этот стиль линии автоматически. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Указывает, назначается ли цвет линии автоматически. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Указывает, видна ли линия. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Определяет соединительные заглавные буквы. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Отображает отрицательное количество ошибок, если тип полосы ошибок — Пользовательский. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Представляет положительную величину ошибки, когда тип полосы ошибок — Пользовательский. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Указывает, форматируются ли полосы ошибок с помощью T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Представляет стиль линии. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Получает и устанавливает цвет темы. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Возвращает или задает степень прозрачности линии в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Представляет тип суммы полосы ошибок. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Получает или задает[`WeightType`](../../aspose.cells.drawing/weighttype) линии. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Получает или задает вес линии в пунктах. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Получает или задает вес линии в пикселях. |

### Примеры

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Смотрите также

* class [Line](../../aspose.cells.drawing/line)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
