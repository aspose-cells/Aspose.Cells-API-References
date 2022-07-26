---
title: SparklineGroup
second_title: Aspose.Cells för .NET API-referens
description: Sparkline./sparkline är organiserad i sparkline-grupp. En SparklineGroup innehåller ett variabelt antal sparkline-objekt. En sparkline-grupp anger typ visningsinställningar och axelinställningar för sparklines.
type: docs
weight: 880
url: /sv/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline) är organiserad i sparkline-grupp. En SparklineGroup innehåller ett variabelt antal sparkline-objekt. En sparkline-grupp anger typ, visningsinställningar och axelinställningar för sparklines.

```csharp
public class SparklineGroup
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden) { get; set; } | Indikerar om data ska visas i dolda rader och kolumner. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor) { get; set; } | Hämtar och ställer in färgen på den första datapunkten i sparklinegruppen. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor) { get; set; } | Hämtar och ställer in färgen på de högsta datapunkterna i sparklinegruppen. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor) { get; set; } | Hämtar och ställer in färgen på den horisontella axeln i sparklinegruppen. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange) { get; set; } | Representerar intervallet som innehåller datumvärdena för sparkline-data. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor) { get; set; } | Hämtar och ställer in färgen på den sista datapunkten i sparklinegruppen. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight) { get; set; } | Hämtar och ställer in linjevikten i varje linje sparkline i sparklinegruppen, i enheten för poäng. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor) { get; set; } | Hämtar och ställer in färgen på de lägsta datapunkterna i sparklinegruppen. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor) { get; set; } | Hämtar och ställer in färgen på punkterna i varje linje sparkline i sparklinegruppen. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor) { get; set; } | Hämtar och ställer in färgen på de negativa värdena på sparklinegruppen. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype) { get; set; } | Indikerar hur tomma celler plottas. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft) { get; set; } | Indikerar om plotdata är från höger till vänster. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle) { get; set; } | Hämtar och ställer in den förinställda stiltypen för sparklinegruppen. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor) { get; set; } | Hämtar och ställer in färgen på sparklines i sparklinegruppen. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint) { get; set; } | Indikerar om den första datapunkten i sparklinegruppen ska markeras. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint) { get; set; } | Indikerar om de högsta punkterna med data i sparklinegruppen ska markeras. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis) { get; set; } | Indikerar om gnistlinjens horisontella axel ska visas. Den horisontella axeln visas om gnistlinjen har data som korsar nollaxeln. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint) { get; set; } | Indikerar om den sista punkten med data i sparklinegruppen ska markeras. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint) { get; set; } | Indikerar om de lägsta datapunkterna i sparklinegruppen ska markeras. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers) { get; set; } | Indikerar om varje punkt i varje linje sparkline i sparklinegruppen ska markeras. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints) { get; set; } | Indikerar om de negativa värdena på sparklinegruppen ska markeras med en annan färg eller markör. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection) { get; } | Får[`SparklineCollection`](./sparklinecollection) objekt för sparkline-gruppen. |
| [Type](../../aspose.cells.charts/sparklinegroup/type) { get; set; } | Indikerar sparkline-typen för sparklinegruppen. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue) { get; set; } | Hämtar och ställer in det anpassade maxvärdet för den vertikala axeln. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype) { get; set; } | Representerar den vertikala axelns maximala värdetyp. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue) { get; set; } | Hämtar och ställer in det anpassade minimivärdet för den vertikala axeln. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype) { get; set; } | Representerar den vertikala axelns minsta värdetyp. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges)(string, bool, CellArea) | Återställer dataintervallet och platsintervallet för sparklinegruppen. Den här metoden rensar ursprungliga sparkline-objekt i gruppen och skapar nya sparkline-objekt för de nya intervallen. |

### Exempel

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Definiera CellArea
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;
 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 // Skapa CellsColor
 CellsColor clr = book.CreateCellsColor();
 clr.Color = Color.Orange;
 group.SeriesColor = clr;

 // set de högsta punkterna färgas gröna och de låga punkterna är färgade röda
 group.ShowHighPoint = true;
 group.ShowLowPoint = true;
 group.HighPointColor.Color = Color.Green;
 group.LowPointColor.Color = Color.Red;
 // ställ in linjevikt 
 group.LineWeight = 1.0;
 book.Save("output.xlsx", SaveFormat.Xlsx);
```

### Se även

* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
