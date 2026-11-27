---
title: "Klass Chart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Chart-klass. Inkapslar objektet som representerar ett enskilt Excel-diagram."
type: docs
url: /sv/net/aspose.cells.charts/chart/
---
## Chart class

Inkapslar objektet som representerar ett enskilt Excel-diagram.

```csharp
public class Chart
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Hämtar den faktiska storleken på diagrammet i pixelenheter. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | Sant om Microsoft Excel skalar ett 3‑D‑diagram så att det är närmare i storlek till motsvarande 2‑D‑diagram. Egenskapen RightAngleAxes måste vara True. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Returnerar ett [`Walls`](./walls/)‑objekt som representerar bakväggen på ett 3‑D‑diagram. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Hämtar diagrammets X‑axel. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Hämtar diagramområdet i kalkylbladet. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Representerar diagrammets datatabell. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Representerar chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Anger om #N/A ska visas som ett tomt värde. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Representerar höjden på 3‑D‑diagramvyn, i grader. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Hämtar en [`SeriesCollection`](../seriescollection/)‑samling som representerar de dataserier som filtreras i diagrammet. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Hämtar eller anger vinkeln på den första sektorn i ett cirkeldiagram eller donutdiagram, i grader (medurs från vertikal). Gäller endast cirkel-, 3‑D‑cirkeldiagram och donutdiagram, 0 till 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Returnerar ett [`Floor`](./floor/)‑objekt som representerar väggarna i ett 3‑D‑diagram. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Hämtar eller anger avståndet mellan dataserierna i ett 3‑D‑diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Anger om fältknapparna för pivottabell-diagram ska döljas endast när diagrammet är ett PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Anger om diagrammet är ett 3d-diagram. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Hämtar eller anger ett värde som indikerar om diagramområdet har rektangulära hörn. Standard är true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Hämtar diagrammets förklaring. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Hämtar linjen. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Hämtar och anger namnet på diagrammet. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Hämtar en [`SeriesCollection`](../seriescollection/) samling som representerar dataserierna i diagrammet. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Representerar sidinställningsbeskrivningen i detta diagram. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Returnerar eller anger perspektivet för den tredimensionella diagramvyn. Måste vara mellan 0 och 100. Denna egenskap ignoreras om egenskapen RightAngleAxes är True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Anger pivotkontrollerna som visas i diagrammet |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Representerar hur diagrammet är fäst vid cellerna under det. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Hämtar diagrammets plotområde som inkluderar axelns tick‑etiketter. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Hämtar och anger om plotten ska göras per rad eller kolumn. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Hämtar och anger hur tomma celler ska plottas. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Anger om endast synliga celler ska plottas. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Anger om endast synliga celler ska plottas. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Hämtar och anger den utskrivna diagramstorleken. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | True om diagramaxlarna är vinkelräta. Gäller endast för 3‑D-diagram (förutom Column3D och 3‑D-pie-diagram). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Representerar rotationen av 3‑D-diagramvyn (rotationen av plotområdet runt z‑axeln, i grader). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Hämtar diagrammets andra X‑axel. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Hämtar diagrammets andra Y‑axel. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Hämtar diagrammets serieaxel. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Returnerar alla ritningsformer i detta diagram. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Hämtar eller anger ett värde som indikerar om diagrammet visar en datatabell. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Hämtar eller anger ett värde som indikerar om diagrammets förklaring ska visas. Standard är true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Returnerar ett [`Walls`](./walls/)‑objekt som representerar sidoväggen i ett 3‑D‑diagram. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | Sant om Microsoft Excel ändrar diagrammets storlek så att den matchar storleken på diagrambladets fönster. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Hämtar och anger den inbyggda stilen. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Hämtar diagrammets undertitel. Gäller endast ODS‑filer. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Hämtar diagrammets titel. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Hämtar eller anger diagrammets typ. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Hämtar diagrammets Y‑axel. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Returnerar ett [`Walls`](./walls/)‑objekt som representerar väggarna i ett 3‑D‑diagram. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | Sant om rutnät ritas tvådimensionellt på ett 3‑D‑diagram. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Hämtar kalkylbladet som innehåller detta diagram. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner tilldelas automatiskt. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Beräknar den anpassade positionen för plotområdet och axlarna om deras positioner tilldelas automatiskt, med Diagramberäkningsalternativ. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Ändra diagramtyp med en förinställd mall. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Hämtar diagrammets faktiska storlek i pixelenheter. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Hämtar diagrammets datakällintervall. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Returnerar vilka axlar som finns i diagrammet. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Returnerar om cellen som diagrammet refererar till. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Detekterar om diagrammets datakälla har ändrats. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Returnerar om cellen refereras av diagrammet. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Flyttar diagrammet till en angiven plats. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Uppdaterar diagrammets data från pivottabell. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Anger dataintervall för ett diagram. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Byter rad/kolumn. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Hämtar ett 32‑bit `Bitmap`‑objekt av diagrammet. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Hämtar ett 32‑bit `Bitmap`‑objekt av diagrammet. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Quality‑attribut ignoreras. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Skapar diagrammets bild och sparar den till en fil. Filnamnets filändelse bestämmer bildens format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Skapar diagrammets bild och sparar den till en ström i det angivna formatet. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Skapar diagrammets bild och sparar den till en ström i det angivna formatet. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Skapar diagrammets bild och sparar den till en ström i det angivna formatet. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Skapar diagrammets bild och sparar den till en ström i Jpeg-format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Skapar diagrammets bild och sparar den till en fil i det angivna formatet. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Skapar diagrammets bild och sparar den till en fil. Filnamnets filändelse bestämmer bildens format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Skapar diagrammets bild och sparar den till en fil i den angivna bildtypen. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Skapar diagrammets bild och sparar den till en fil i Jpeg-format. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Skapar diagrammets PDF och sparar den till en ström. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Sparar diagrammet till en pdf-fil. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Skapar diagrammets pdf och sparar den till en ström. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Sparar diagrammet till en pdf-fil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:B4", true);

            // Ange diagrammets egenskaper
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Anpassa diagrammets utseende
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Anpassa diagrammets axlar
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Anpassa diagrammets förklaring
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Anpassa diagrammets plotområde
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Anpassa diagrammets diagramområde
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Spara arbetsboken
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


