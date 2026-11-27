---
title: "Klassen Series"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Series-klass. Inkapslar objektet som representerar en enskild dataserie i ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/series/
---
## Series class

Inkapslar objektet som representerar en enskild dataserie i ett diagram.

```csharp
public class Series
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Representerar bakgrundsområdet för Series-objektet. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Hämtar eller anger 3D-formtypen som används med 3‑D stapel- eller kolumndiagram. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Representerar kanten på ett Series-objekt. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Hämtar eller anger skalningsfaktorn för bubblor i den angivna diagramgruppen. Den kan vara ett heltal mellan 0 (noll) och 300, motsvarande en procentsats av standardstorleken. Gäller endast för bubbeldiagram. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Hämtar eller anger bubbelstorleksvärdena för diagramserien. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Hämtar de cachade kategorivärdena för serien |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Hämtar de cachade värdena för serien |
| [CategoryValues](../../aspose.cells.charts/series/categoryvalues/) { get; } | Hämtar de faktiska kategorivärdena som används för att plotta varje punkt i denna serie i diagrammet. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Hämtar antalet datavärden. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Representerar DataLabels-objektet för den angivna ASeries. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Hämtar seriens namn som visas i diagramgrafen. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentsats av diagrammets storlek, mellan 10 och 90 procent. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Returnerar ett [`DropBars`](../dropbars/)‑objekt som representerar nedstaplar i ett linjediagram. Gäller endast för linjediagram. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Returnerar ett [`Line`](../../aspose.cells.drawing/line/)‑objekt som representerar droplinjer för en serie i linje- eller områdesdiagram. Gäller endast för linje- eller områdesdiagram. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | Avståndet för ett öppet pajsegment från centrum av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Hämtar eller anger vinkeln för den första paj- eller donutskivan, i grader (medurs från vertikal). Gäller endast för paj-, 3‑D-paj- och donutdiagram, med värden från 0 till 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | Sant om serien har ett tredimensionellt utseende. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | Sant om diagrammet har droplinjer. Gäller endast för linje- eller områdesdiagram. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | Sant om linjediagrammet har hög-låg-linjer. Gäller endast för linjediagram. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | Sant om serien har ledarlinjer. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | Sant om ett radardiagram har kategoriska axelrubriker. Gäller endast radardiagram. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna. Gäller endast staplade kolumndiagram, stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | Sant om ett linjediagram har upp- och nedåtbalkar. Gäller endast linjediagram. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Returnerar ett HiLoLines-objekt som representerar hög-låg-linjerna för en serie i ett linjediagram. Gäller endast linjediagram. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Anger om tröskelvärdet är automatiskt. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Representerar om färgen på punkterna varierar. Diagrammet måste innehålla endast en serie eller så är diagrammet ett cirkeldiagram. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Anger om serien är markerad eller filtrerad. Sant indikerar att serien är filtrerad och den kommer inte att visas i diagrammet. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Anger om datakällan är vertikal. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Representerar layoutens egenskaper. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Representerar ledarlinjer i ett diagram. Ledarlinjer kopplar datamärkningar till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enskild ledarlinje. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Hämtar legendposten för denna serie. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Hämtar [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Hämtar eller anger namnet på dataserien. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Anger hur staplar och kolumner placeras. Kan vara ett värde mellan -100 och 100. Gäller endast 2‑D stapeldiagram och 2‑D kolumndiagram. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Anger om denna serie plottas på den sekundära värdeaxeln. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Hämtar samlingen av punkter i en serie i ett diagram. |
| [PointValues](../../aspose.cells.charts/series/pointvalues/) { get; } | Hämtar de faktiska värdena som används för att plotta varje punkt i denna serie i diagrammet. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Returnerar eller anger storleken på den sekundära sektionen i antingen ett Pie of Pie-diagram eller ett Bar of Pie-diagram, som en procentandel av storleken på den primära pajen. Kan vara ett värde mellan 5 och 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Returnerar ett SeriesLines-objekt som representerar serielinjerna för ett staplat stapeldiagram eller ett staplat kolumndiagram. Gäller endast staplade stapeldiagram och staplade kolumndiagram. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | Sant om serien har en skugga. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Hämtar [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/)‑objektet som innehåller de visuella formegenskaperna för serien. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | Sant om negativa bubblor visas för diagramgruppen. Giltigt endast för bubbeldiagram. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Hämtar eller anger vad bubbelstorleken representerar i ett bubbeldiagram. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Representerar kurvutjämning. Sant om kurvutjämning är aktiverad för linjediagram eller spridningsdiagram. Gäller endast linjediagram och spridningsdiagram med linjer. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Returnerar eller anger ett värde som bestämmer vilka datapunkter som finns i den andra pajen eller stapeln i ett Pie of Pie- eller Bar of Pie-diagram. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln på ett paj‑av‑paj‑ eller stapel‑av‑paj‑diagram. |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Returnerar alla trendlinjer för denna serie. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Hämtar eller anger en dataserietyp. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Returnerar ett DropBars‑objekt som representerar uppåtriktade staplar i ett linjediagram. Gäller endast linjediagram. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Representerar Y‑värdena för denna diagramserie. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Representerar formatkoden för Values NumberList. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Representerar X‑riktningens felstapel för serien. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Representerar X‑värdena för denna diagramserie. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Representerar formatkoden för X Values' NumberList. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Representerar Y‑riktningens felstapel för serien. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Flyttar serien upp eller ner. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesDemo
    {
        public static void SeriesExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
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

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) i diagrammet från cellen "A1" till "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Anger datakällan för kategoridata i NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Åtkomst till serien
            Series series = chart.NSeries[seriesIndex];

            // Ställer in värdena för serien
            series.Values = "=B1:B4";
            // Ändra diagramtypen för serien
            series.Type = ChartType.Line;
            // Ställa in markörens egenskaper
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Ställer in ytterligare egenskaper
            series.Name = "First Series";
            series.IsFiltered = false;
            series.ValuesFormatCode = "0.00";
            series.XValues = "=A1:A4";
            series.BubbleSizes = "=B1:B4";
            series.Smooth = true;
            series.Shadow = true;
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;
            series.PlotOnSecondAxis = false;
            series.HasHiLoLines = false;
            series.HasSeriesLines = false;
            series.HasDropLines = false;
            series.HasUpDownBars = false;
            series.IsColorVaried = false;
            series.GapWidth = 150;
            series.FirstSliceAngle = 45;
            series.Overlap = 0;
            series.SecondPlotSize = 100;
            series.SplitType = ChartSplitType.Position;
            series.SplitValue = 10.0;
            series.BubbleScale = 100;
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;
            series.ShowNegativeBubbles = true;
            series.DoughnutHoleSize = 50;
            series.Explosion = 10;
            series.HasRadarAxisLabels = false;
            series.HasLeaderLines = true;

            // Sparar Excel-filen
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


