---
title: "Klasse Series"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Series Klasse. Kapselt das Objekt, das eine einzelne Datenreihe in einem Diagramm darstellt"
type: docs
url: /de/net/aspose.cells.charts/series/
---
## Series class

Kapselt das Objekt, das eine einzelne Datenserie in einem Diagramm darstellt.

```csharp
public class Series
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area/) { get; } | Stellt den Hintergrundbereich des Series-Objekts dar. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype/) { get; set; } | Liest oder legt den 3D-Formtyp fest, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird. |
| [Border](../../aspose.cells.charts/series/border/) { get; } | Stellt die Rahmenlinie eines Series-Objekts dar. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale/) { get; set; } | Liest oder legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest. Er kann ein ganzzahliger Wert von 0 (null) bis 300 sein, was einem Prozentsatz der Standardgröße entspricht. Gilt nur für Blasendiagramme. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes/) { get; set; } | Liest oder legt die Blasengrößenwerte der Diagrammreihe fest. |
| [CachedCategoryValues](../../aspose.cells.charts/series/cachedcategoryvalues/) { get; } | (**Obsolete.**) Liest die zwischengespeicherten Kategorienwerte für die Reihe |
| [CachedValues](../../aspose.cells.charts/series/cachedvalues/) { get; } | (**Obsolete.**) Liest die zwischengespeicherten Werte für die Reihe |
| [CategoryValues](../../aspose.cells.charts/series/categoryvalues/) { get; } | Liest die tatsächlichen Kategorienwerte, die zum Plotten jedes Punktes dieser Reihe im Diagramm verwendet werden. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues/) { get; } | Liest die Anzahl der Datenwerte. |
| [DataLabels](../../aspose.cells.charts/series/datalabels/) { get; } | Stellt das DataLabels-Objekt für die angegebene ASeries dar. |
| [DisplayName](../../aspose.cells.charts/series/displayname/) { get; } | Liest den Namen der Reihe, der im Diagramm angezeigt wird. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize/) { get; set; } | Liefert oder legt die Größe des Lochs in einer Donut‑Diagrammgruppe fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße ausgedrückt, zwischen 10 % und 90 %. |
| [DownBars](../../aspose.cells.charts/series/downbars/) { get; } | Liefert ein [`DropBars`](../dropbars/) Objekt, das die Abwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [DropLines](../../aspose.cells.charts/series/droplines/) { get; } | Liefert ein [`Line`](../../aspose.cells.drawing/line/) Objekt, das die Drop‑Lines für eine Reihe im Liniendiagramm oder Flächendiagramm darstellt. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [Explosion](../../aspose.cells.charts/series/explosion/) { get; set; } | Der Abstand eines offenen Kuchenstücks vom Mittelpunkt des Kreisdiagramms wird als Prozentsatz des Durchmessers des Kreises angegeben. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle/) { get; set; } | Liest oder legt den Winkel des ersten Kuchen‑ oder Donutscheibens in Grad fest (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen-, 3‑D‑Kuchen‑ und Donutdiagramme, mit Werten von 0 bis 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth/) { get; set; } | Gibt den Abstand zwischen Balken‑ oder Spalten‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Spaltenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect/) { get; set; } | True, wenn die Reihe ein dreidimensionales Erscheinungsbild hat. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines/) { get; set; } | True, wenn das Diagramm Drop‑Lines hat. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines/) { get; set; } | True, wenn das Liniendiagramm Hoch‑Tief‑Linien hat. Gilt nur für Liniendiagramme. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines/) { get; set; } | True, wenn die Reihe Führungs‑Linien hat. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels/) { get; set; } | True, wenn ein Radar‑Diagramm Kategorienachsen‑Beschriftungen hat. Gilt nur für Radar‑Diagramme. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines/) { get; set; } | True, wenn ein gestapeltes Säulen‑ oder Balkendiagramm Serienlinien hat oder ein Pie‑of‑Pie‑ bzw. Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulendiagramme, Balkendiagramme, Pie‑of‑Pie‑Diagramme oder Bar‑of‑Pie‑Diagramme. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars/) { get; set; } | True, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. Gilt nur für Liniendiagramme. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines/) { get; } | Gibt ein HiLoLines-Objekt zurück, das die Hoch‑Tief‑Linien für eine Serie in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit/) { get; } | Gibt an, ob der Schwellenwert automatisch ist. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried/) { get; set; } | Stellt dar, ob die Farbe der Punkte variiert. Das Diagramm muss nur eine Serie enthalten oder ein Kreisdiagramm sein. |
| [IsFiltered](../../aspose.cells.charts/series/isfiltered/) { get; set; } | Gibt an, ob die Serie ausgewählt oder gefiltert ist. Wahr bedeutet, dass diese Serie gefiltert ist und nicht im Diagramm angezeigt wird. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues/) { get; } | Gibt an, ob die Datenquelle vertikal ist. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties/) { get; } | Stellt die Eigenschaften des Layouts dar. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines/) { get; } | Stellt Führungs‑Linien in einem Diagramm dar. Führungs‑Linien verbinden Datenbeschriftungen mit Datenpunkten. Dieses Objekt ist keine Sammlung; es gibt kein Objekt, das eine einzelne Führungs‑Linie darstellt. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry/) { get; } | Liefert den Legendeintrag für diese Serie. |
| [Marker](../../aspose.cells.charts/series/marker/) { get; } | Liefert das [`marker`](./marker/). |
| [Name](../../aspose.cells.charts/series/name/) { get; set; } | Liest oder setzt den Namen der Datenserie. |
| [Overlap](../../aspose.cells.charts/series/overlap/) { get; set; } | Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen -100 und 100 sein. Gilt nur für 2‑D‑Balken‑ und 2‑D‑Säulendiagramme. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis/) { get; set; } | Gibt an, ob diese Serie auf der sekundären Wertachse dargestellt wird. |
| [Points](../../aspose.cells.charts/series/points/) { get; } | Liefert die Sammlung von Punkten einer Serie in einem Diagramm. |
| [PointValues](../../aspose.cells.charts/series/pointvalues/) { get; } | Liefert die tatsächlichen Werte, die zum Plotten jedes Punktes dieser Serie im Diagramm verwendet werden. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize/) { get; set; } | Gibt die Größe des sekundären Abschnitts eines Kreis‑in‑Kreis‑Diagramms oder eines Balken‑in‑Kreis‑Diagramms als Prozentsatz der Größe des primären Kreises zurück oder setzt sie. Kann ein Wert von 5 bis 200 sein. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines/) { get; } | Gibt ein SeriesLines-Objekt zurück, das die Serienlinien für ein gestapeltes Balken‑ oder Säulendiagramm darstellt. Gilt nur für gestapelte Balken‑ und Säulendiagramme. |
| [Shadow](../../aspose.cells.charts/series/shadow/) { get; set; } | Wahr, wenn die Serie einen Schatten hat. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties/) { get; } | Liefert das [`ShapePropertyCollection`](../../aspose.cells.drawing/shapepropertycollection/)‑Objekt, das die visuellen Formeigenschaften der Serie enthält. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles/) { get; set; } | Wahr, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Gültig nur für Blasendiagramme. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents/) { get; set; } | Liest oder setzt, was die Blasengröße in einem Blasendiagramm darstellt. |
| [Smooth](../../aspose.cells.charts/series/smooth/) { get; set; } | Stellt die Kurvenglättung dar. Wahr, wenn die Kurvenglättung für ein Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien. |
| [SplitType](../../aspose.cells.charts/series/splittype/) { get; set; } | Gibt einen Wert zurück oder setzt ihn, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue/) { get; set; } | Gibt einen Wert zurück oder setzt ihn, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [TrendLines](../../aspose.cells.charts/series/trendlines/) { get; } | Gibt alle Trendlinien dieser Serie zurück. |
| [Type](../../aspose.cells.charts/series/type/) { get; set; } | Liest oder setzt den Typ einer Datenserie. |
| [UpBars](../../aspose.cells.charts/series/upbars/) { get; } | Gibt ein DropBars-Objekt zurück, das die Aufwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [Values](../../aspose.cells.charts/series/values/) { get; set; } | Stellt die Y‑Werte dieser Diagrammserie dar. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode/) { get; set; } | Stellt den Formatcode der Werte‑NumberList dar. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar/) { get; } | Stellt den X‑Richtungs-Fehlerbalken der Serie dar. |
| [XValues](../../aspose.cells.charts/series/xvalues/) { get; set; } | Stellt die X‑Werte dieser Diagrammserie dar. |
| [XValuesFormatCode](../../aspose.cells.charts/series/xvaluesformatcode/) { get; set; } | Stellt den Formatcode der X‑Werte‑NumberList dar. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar/) { get; } | Stellt den Y‑Richtungs-Fehlerbalken der Serie dar. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move/)(int) | Verschiebt die Serie nach oben oder unten. |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            // Ein neues Arbeitsblatt zum Excel-Objekt hinzufügen
            int sheetIndex = workbook.Worksheets.Add();
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hinzufügen von Beispielwerten zu Zellen
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

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Festlegen der Datenquelle für die Kategoriedaten von NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Zugriff auf die Serie
            Series series = chart.NSeries[seriesIndex];

            // Festlegen der Werte der Serie
            series.Values = "=B1:B4";
            // Ändern des Diagrammtyps der Serie
            series.Type = ChartType.Line;
            // Festlegen von Markereigenschaften
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Zusätzliche Eigenschaften festlegen
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

            // Die Excel-Datei speichern
            workbook.Save("SeriesExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


