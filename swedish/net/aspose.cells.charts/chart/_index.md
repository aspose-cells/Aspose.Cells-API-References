---
title: Chart
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar ett enda Excel-diagram.
type: docs
weight: 430
url: /sv/net/aspose.cells.charts/chart/
---
## Chart class

Kapslar in objektet som representerar ett enda Excel-diagram.

```csharp
public class Chart
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | Sant om Microsoft Excel skalar ett 3D-diagram så att det är närmare motsvarande 2D-diagram. Egenskapen RightAngleAxes måste vara True. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Returnerar en[`Walls`](./walls) objekt som representerar bakväggen i ett 3D-diagram. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Hämtar diagrammets X-axel. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Hämtar diagramområdet i kalkylbladet. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Representerar diagramdatatabellen. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | Representerar diagramformen; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Representerar djupet på ett 3D-diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Indikerar om #N/A visas som tomt värde. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Representerar höjden av 3D-sjökortsvyn, i grader. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Hämtar eller ställer in vinkeln för det första cirkeldiagrammet eller munkdiagrammet, i grader (medsols från lodrät). Gäller endast paj-, 3D-paj- och munkdiagram, 0 till 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Returnerar en[`Floor`](./floor) objekt som representerar väggarna i ett 3D-diagram. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Hämtar eller ställer in avståndet mellan dataserierna i ett 3D-diagram, i procent av markörens bredd. Värdet på den här egenskapen måste vara mellan 0 och 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Returnerar eller ställer in utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapel- eller kolumnbredden. Värdet på den här egenskapen måste vara mellan 0 och 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Returnerar eller ställer in höjden på ett 3D-diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Indikerar om knapparna för pivotdiagramfältet endast döljs när diagrammet är PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Indikerar om diagrammet är ett 3d-diagram. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Hämtar eller ställer in ett värde som anger om diagramområdet är rektangulärt hörn. Standard är sant. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Hämtar diagramförklaringen. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Får linjen. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Hämtar och ställer in namnet på diagrammet. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | Får en[`SeriesCollection`](../seriescollection) samling som representerar dataserien i diagrammet. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Representerar sidkonfigurationsbeskrivningen i detta diagram. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Returnerar eller ställer in perspektivet för 3D-diagramvyn. Måste vara mellan 0 och 100. Den här egenskapen ignoreras om egenskapen RightAngleAxes är True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Anger pivotkontrollerna som visas på diagrammet |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | Källan är pivottabellens data. Om PivotSource inte är tom är diagrammet PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Representerar hur diagrammet är fäst vid cellerna under det. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Hämtar diagrammets plotområde som inkluderar axelmarkeringsetiketter. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Hämtar och ställer in om plottning efter rad eller kolumn. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Hämtar och ställer in hur de tomma cellerna ska plottas. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Indikerar om endast plotta synliga celler. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Hämtar och ställer in den utskrivna diagramstorleken. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Sant om diagrammets axlar är i rät vinkel. Gäller endast för 3D-diagram (förutom Column3D och 3-D cirkeldiagram). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Representerar rotationen av 3D-diagramvyn (rotationen av plotområdet runt z-axeln, i grader). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Hämtar diagrammets andra X-axel. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Hämtar diagrammets andra Y-axel. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Hämtar diagrammets serieaxel. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Returnerar alla ritningsformer i detta diagram. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Hämtar eller ställer in ett värde som anger om diagrammet visar en datatabell. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Hämtar eller ställer in ett värde som anger om diagramförklaringen kommer att visas. Standard är sant. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Returnerar en[`Walls`](./walls)objekt som representerar sidoväggen på ett 3D-diagram. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Sant om Microsoft Excel ändrar storleken på diagrammet för att matcha storleken på diagrambladets fönster. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Hämtar och ställer in den inbyggda stilen. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Hämtar diagrammets underrubrik. Endast för fil i ODS-format. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Hämtar diagrammets titel. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Hämtar eller ställer in ett diagrams typ. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Hämtar diagrammets Y-axel. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Returnerar en[`Walls`](./walls) objekt som representerar väggarna i ett 3D-diagram. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Sant om rutnätslinjer ritas tvådimensionellt på ett 3D-diagram. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Hämtar kalkylbladet som innehåller detta diagram. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Beräknar den anpassade positionen för plottarean, axlar om positionen för dem är automatiskt tilldelad. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Hämtar den faktiska storleken på diagrammet i enhet pixlar. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Hämtar datakällans intervall för diagrammet. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Returnerar vilka axlar som finns i diagrammet. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Upptäcker om ett diagrams datakälla har ändrats. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Flyttar diagrammet till en angiven plats. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Uppdaterar pivotdiagrammets data från dess pivotdatakälla. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Anger dataintervall för ett diagram. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Byter rad/kolumn. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Får en 32-bitars`Bitmapp` objekt i diagrammet. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Får en 32-bitars`Bitmapp` objekt i diagrammet. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression och ImageOrPrintOptions.Kvalitetsattribut ignoreras. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Skapar diagrambilden och sparar den i en fil. Filnamnstillägget bestämmer formatet på bilden. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Skapar diagrambilden och sparar den i en ström i angivet format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Skapar diagrambilden och sparar den i en ström i angivet format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Skapar diagrambilden och sparar den i en ström i Jpeg-format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Skapar diagrambilden och sparar den i en fil. Filnamnstillägget bestämmer formatet på bilden. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Skapar diagrambilden och sparar den i en fil i angiven bildtyp. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Skapar diagrambilden och sparar den i en fil i Jpeg-format. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Skapar diagrammets pdf och sparar det i en ström. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Sparar diagrammet i en pdf-fil. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Skapar diagrammets pdf och sparar det i en ström. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Sparar diagrammet i en pdf-fil. |

### Exempel

```csharp
[C#]

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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Se även

* namnutrymme [Aspose.Cells.Charts](../../aspose.cells.charts)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
