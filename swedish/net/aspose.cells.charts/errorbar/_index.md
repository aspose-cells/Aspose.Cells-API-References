---
title: ErrorBar
second_title: Aspose.Cells för .NET API-referens
description: Representerar felfältet för dataserien.
type: docs
weight: 630
url: /sv/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Representerar felfältet för dataserien.

```csharp
public class ErrorBar : Line
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Representerar mängden felfält.  Beloppet måste vara större än eller lika med noll. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Anger längden på pilspetsen för början av en linje. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Anger bredden på pilspetsen för början av en linje. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Anger en pilspets för början av en rad. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Anger slutbeteckningar. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | RepresenterarColor av linjen. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Anger den sammansatta linjetypen |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Anger strecklinjetypen |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Representerar felfältets visningstyp. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Anger längden på pilspetsen för slutet av en linje. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Anger bredden på pilspetsen för slutet av en linje. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Anger en pilspets för slutet av en rad. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Hämtar eller ställer in formattyp. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Representerar gradientfyllning. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indikerar om denna linjestil är automatiskt tilldelad. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indikerar om färgen på linjen är automatiskt tilldelad. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Representerar om linjen är synlig. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Anger sammanfogningskapslarna. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Representerar negativt felbelopp när felstapeltypen är Custom. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Representerar positivt felmängd när felstapeltypen är Custom. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Indikerar om formateringsfelstaplar med en T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Representerar stilen på linjen. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Hämtar och ställer in temafärgen. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Returnerar eller ställer in graden av genomskinlighet för linjen som ett värde från 0,0 (ogenomskinlig) till 1,0 (ren). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Representerar felstapelbeloppstyp. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Hämtar eller ställer in[`WeightType`](../../aspose.cells.drawing/weighttype) av linjen. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Hämtar eller ställer in linjens vikt i poängenhet. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Hämtar eller ställer in linjens vikt i pixelenhet. |

### Exempel

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

### Se även

* class [Line](../../aspose.cells.drawing/line)
* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
