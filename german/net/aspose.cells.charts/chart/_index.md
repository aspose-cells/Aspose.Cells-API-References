---
title: Chart
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das ein einzelnes Excel-Diagramm darstellt.
type: docs
weight: 430
url: /de/net/aspose.cells.charts/chart/
---
## Chart class

Kapselt das Objekt, das ein einzelnes Excel-Diagramm darstellt.

```csharp
public class Chart
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | True, wenn Microsoft Excel ein 3D-Diagramm so skaliert, dass es in der Größe näher an dem entsprechenden 2D-Diagramm liegt. Die RightAngleAxes-Eigenschaft muss True sein. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Gibt a zurück[`Walls`](./walls) Objekt, das die Rückwand eines 3D-Diagramms darstellt. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Ruft die X-Achse des Diagramms ab. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Ruft den Diagrammbereich im Arbeitsblatt ab. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Repräsentiert die Diagrammdatentabelle. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | stellt die Diagrammform dar; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Repräsentiert die Tiefe eines 3D-Diagramms als Prozentsatz der Diagrammbreite (zwischen 20 und 2000 Prozent). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Gibt an, ob #N/A als Leerwert angezeigt wird. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Stellt die Höhe der 3D-Kartenansicht in Grad dar. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Liest oder setzt den Winkel des ersten Torten- oder Doughnut-Diagramms in Grad (im Uhrzeigersinn von der Vertikalen). Gilt nur für Kreis-, 3D-Kreis- und Ringdiagramme, 0 bis 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Gibt a zurück[`Floor`](./floor) Objekt, das die Wände eines 3D-Diagramms darstellt. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Ruft den Abstand zwischen den Datenreihen in einem 3D-Diagramm als Prozentsatz der Markierungsbreite ab oder legt ihn fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Gibt den Abstand zwischen Balken- oder Spaltenclustern als Prozentsatz der Balken- oder Spaltenbreite zurück oder legt ihn fest. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Gibt die Höhe eines 3D-Diagramms als Prozentsatz der Diagrammbreite zurück oder legt sie fest (zwischen 5 und 500 Prozent). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Gibt an, ob die Feldschaltflächen des Pivot-Diagramms nur ausgeblendet werden, wenn das Diagramm ein PivotChart ist. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Gibt an, ob das Diagramm ein 3D-Diagramm ist. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Diagrammbereich rechteckig ist. Der Standardwert ist wahr. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Ruft die Diagrammlegende ab. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Ruft die Leitung ab. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Ruft den Namen des Diagramms ab und legt ihn fest. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | erhält a[`SeriesCollection`](../seriescollection) Sammlung, die die Datenreihen im Diagramm darstellt. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Stellt die Beschreibung der Seiteneinrichtung in diesem Diagramm dar. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Gibt die Perspektive für die 3D-Kartenansicht zurück oder legt sie fest. Muss zwischen 0 und 100 liegen. Diese Eigenschaft wird ignoriert, wenn die Eigenschaft RightAngleAxes True ist. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Gibt die Pivot-Steuerelemente an, die auf dem Diagramm erscheinen |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | Die Quelle sind die Daten der PivotTable. Wenn PivotSource nicht leer ist, ist das Diagramm PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Stellt dar, wie das Diagramm mit den darunter liegenden Zellen verbunden ist. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Ruft den Plotbereich des Diagramms ab, der Achsenstrichbeschriftungen enthält. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Ruft ab und legt fest, ob nach Zeile oder Spalte gezeichnet wird. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Ruft ab und legt fest, wie die leeren Zellen geplottet werden. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Gibt an, ob nur sichtbare Zellen gezeichnet werden sollen. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Ruft die gedruckte Diagrammgröße ab und legt sie fest. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Wahr, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3D-Diagramme (außer Column3D- und 3D-Kreisdiagramme). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Stellt die Drehung der 3D-Diagrammansicht dar (die Drehung des Diagrammbereichs um die Z-Achse in Grad). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Ruft die zweite X-Achse des Diagramms ab. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Ruft die zweite Y-Achse des Diagramms ab. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Ruft die Reihenachse des Diagramms ab. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Gibt alle Zeichnungsformen in diesem Diagramm zurück. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist wahr. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Gibt a zurück[`Walls`](./walls)Objekt, das die Seitenwand eines 3D-Diagramms darstellt. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Wahr, wenn Microsoft Excel die Größe des Diagramms an die Größe des Diagrammblattfensters anpasst. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Ruft den integrierten Stil ab und legt ihn fest. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Ruft den Untertitel des Diagramms ab. Nur für Datei im ODS-Format. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Ruft den Titel des Diagramms ab. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Ruft den Typ eines Diagramms ab oder legt ihn fest. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Ruft die Y-Achse des Diagramms ab. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Gibt a zurück[`Walls`](./walls) Objekt, das die Wände eines 3D-Diagramms darstellt. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Wahr, wenn Gitternetzlinien zweidimensional auf einem 3D-Diagramm gezeichnet werden. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Ruft das Arbeitsblatt ab, das dieses Diagramm enthält. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Berechnet die benutzerdefinierte Position des Plotbereichs, Achsen, wenn deren Position automatisch zugewiesen wird. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Ruft die tatsächliche Größe des Diagramms in Pixeleinheiten ab. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Ruft den Datenquellenbereich des Diagramms ab. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Gibt zurück, welche Achsen im Diagramm vorhanden sind. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Erkennt, ob sich die Datenquelle eines Diagramms geändert hat. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Verschiebt das Diagramm an eine bestimmte Position. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Aktualisiert die Daten des Pivot-Diagramms aus seiner Pivot-Datenquelle. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Gibt den Datenbereich für ein Diagramm an. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Wechselt Zeile/Spalte. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Ruft eine 32-Bit-Version ab`Bitmap` Objekt des Diagramms. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Ruft eine 32-Bit-Version ab`Bitmap` Objekt des Diagramms. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression und ImageOrPrintOptions.Quality werden ignoriert. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Erweiterung des Dateinamens bestimmt das Format des Bildes. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Erstellt das Diagrammbild und speichert es in einem Stream im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Erstellt das Diagrammbild und speichert es in einem Stream im JPEG-Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Erweiterung des Dateinamens bestimmt das Format des Bildes. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Erstellt das Diagrammbild und speichert es in einer Datei im JPEG-Format. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Erstellt das Diagramm-PDF und speichert es in einem Stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Speichert das Diagramm in einer PDF-Datei. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Erstellt das Diagramm-PDF und speichert es in einem Stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Speichert das Diagramm in einer PDF-Datei. |

### Beispiele

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

### Siehe auch

* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
