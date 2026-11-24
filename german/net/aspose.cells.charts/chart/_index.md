---
title: "Klasse Chart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Chart‑Klasse. Kapselt das Objekt, das ein einzelnes Excel‑Diagramm darstellt"
type: docs
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
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Gibt die tatsächliche Größe des Diagramms in Pixeln zurück. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | True, wenn Microsoft Excel ein 3‑D‑Diagramm skaliert, sodass es in der Größe dem entsprechenden 2‑D‑Diagramm näher kommt. Die Eigenschaft RightAngleAxes muss True sein. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Gibt ein [`Walls`](./walls/)-Objekt zurück, das die Rückwand eines 3‑D‑Diagramms darstellt. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Liefert die X‑Achse des Diagramms. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Liefert den Diagrammbereich im Arbeitsblatt. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Stellt die Diagrammdatentabelle dar. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Stellt das chartShape dar; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Stellt die Tiefe eines 3‑D‑Diagramms als Prozentsatz der Diagrammbreite dar (zwischen 20 % und 2000 %). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Gibt an, ob #N/A als leerer Wert angezeigt werden soll. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Stellt die Elevation der 3‑D‑Diagrammansicht in Grad dar. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Liefert eine [`SeriesCollection`](../seriescollection/)-Sammlung, die die im Diagramm gefilterten Datenreihen darstellt. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Liefert oder setzt den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments in Grad (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen-, 3‑D‑Kuchen‑ und Donut‑Diagramme, 0 bis 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Gibt ein [`Floor`](./floor/)-Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Liefert oder setzt den Abstand zwischen den Datenreihen in einem 3‑D‑Diagramm als Prozentsatz der Markierungsbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Gibt den Abstand zwischen Balken‑ oder Spalten‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Spaltenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Gibt die Höhe eines 3‑D‑Diagramms zurück oder setzt sie, als Prozentsatz der Diagrammbreite (zwischen 5 % und 500 %). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Gibt an, ob das Diagramm ein 3‑D‑Diagramm ist. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Liefert oder setzt einen Wert, der angibt, ob der Diagrammbereich rechteckige Ecken hat. Standard ist true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Liefert die Diagrammlegende. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Liest die Zeile. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Liest und setzt den Namen des Diagramms. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Liest eine [`SeriesCollection`](../seriescollection/) Sammlung, die die Datenreihen im Diagramm darstellt. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Stellt die Seitenlayoutbeschreibung in diesem Diagramm dar. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Liefert oder setzt die Perspektive für die dreidimensionale Diagrammansicht. Muss zwischen 0 und 100 liegen. Diese Eigenschaft wird ignoriert, wenn die RightAngleAxes‑Eigenschaft True ist. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Gibt die Pivot‑Steuerelemente an, die im Diagramm angezeigt werden. |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | Die Quelle sind die Daten der Pivot‑Tabelle. Wenn PivotSource nicht leer ist, ist das Diagramm ein PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Stellt dar, wie das Diagramm an den darunterliegenden Zellen befestigt ist. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Liest den Zeichenbereich des Diagramms, der Achsenbeschriftungen enthält. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Liest und setzt, ob nach Zeile oder Spalte geplottet wird. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Liest und setzt, wie leere Zellen geplottet werden. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Gibt an, ob nur sichtbare Zellen geplottet werden. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Liest und setzt die Druckgröße des Diagramms. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | True, wenn die Diagrammachsen rechtwinklig sind. Gilt nur für 3‑D‑Diagramme (außer Column3D und 3‑D‑Kreisdiagrammen). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Zeichenbereichs um die Z‑Achse in Grad). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Liest die zweite X‑Achse des Diagramms. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Liest die zweite Y‑Achse des Diagramms. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Liest die Reihen‑Achse des Diagramms. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Liefert alle Zeichenformen in diesem Diagramm. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das Diagramm eine Datentabelle anzeigt. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Liefert ein [`Walls`](./walls/)‑Objekt, das die Seitenwand eines 3‑D‑Diagramms darstellt. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblatt‑Fensters anpasst. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Liest und setzt den integrierten Stil. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Ermittelt den Untertitel des Diagramms. Gilt nur für ODS-Dateien. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Ermittelt den Titel des Diagramms. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Liest oder legt den Diagrammtyp fest. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Ermittelt die Y-Achse des Diagramms. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Gibt ein [`Walls`](./walls/) Objekt zurück, das die Wände eines 3‑D‑Diagramms darstellt. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | True, wenn Rasterlinien zweidimensional in einem 3‑D‑Diagramm gezeichnet werden. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Ermittelt das Arbeitsblatt, das dieses Diagramm enthält. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Berechnet die benutzerdefinierten Positionen des Plotbereichs und der Achsen, wenn deren Positionen automatisch zugewiesen werden. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Berechnet die benutzerdefinierte Position von Plotbereich und Achsen, wenn deren Position automatisch zugewiesen wird, mit Chart Calculate Options. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Diagrammtyp mit einer vordefinierten Vorlage ändern. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Ermittelt die tatsächliche Größe des Diagramms in Pixel. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Ermittelt den Datenquellenbereich des Diagramms. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Gibt zurück, welche Achsen im Diagramm vorhanden sind. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Gibt zurück, ob die vom Diagramm referenzierte Zelle vorhanden ist. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Erkennt, ob sich die Datenquelle eines Diagramms geändert hat. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Gibt zurück, ob die Zelle vom Diagramm referenziert wird. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Verschiebt das Diagramm an einen angegebenen Ort. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Aktualisiert die Diagrammdaten aus der Pivot-Tabelle. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Legt den Datenbereich für ein Diagramm fest. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Vertauscht Zeile/Spalte. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Ermittelt ein 32‑Bit `Bitmap`‑Objekt des Diagramms. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Ermittelt ein 32‑Bit `Bitmap`‑Objekt des Diagramms. Die Attribute `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression und ImageOrPrintOptions.Quality werden ignoriert. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Erstellt das Diagrammbild und speichert es in einen Stream im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Erstellt das Diagrammbild und speichert es in einen Stream im Jpeg-Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Erstellt das Diagrammbild und speichert es in einer Datei. Die Dateierweiterung bestimmt das Bildformat. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Erstellt das Diagrammbild und speichert es in einer Datei im Jpeg-Format. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Erstellt das Diagramm-PDF und speichert es in einen Stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Speichert das Diagramm in einer PDF-Datei. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Erstellt das Diagramm-PDF und speichert es in einen Stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Speichert das Diagramm in einer PDF-Datei. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.SetChartDataRange("A1:B4", true);

            // Diagrammeigenschaften festlegen
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Aussehen des Diagramms anpassen
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Achsen des Diagramms anpassen
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Legende des Diagramms anpassen
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Diagramm-Plotbereich anpassen
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Diagrammbereich anpassen
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


