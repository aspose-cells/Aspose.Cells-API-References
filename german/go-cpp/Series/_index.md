---
title: "Series Klasse"
linktitle: "Series"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Series Klasse. Kapselt das Objekt, das series in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/series/
---

## Series class

Kapselt das Objekt, das eine einzelne Datenserie in einem Diagramm darstellt.

```go

type Series struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsFiltered](./isfiltered/) | Gibt an, ob die Serie ausgewählt oder gefiltert ist. True gibt an, dass diese Serie gefiltert ist und nicht im Diagramm angezeigt wird. |
| [SetIsFiltered](./setisfiltered/) | Gibt an, ob die Serie ausgewählt oder gefiltert ist. True gibt an, dass diese Serie gefiltert ist und nicht im Diagramm angezeigt wird. |
| [GetLayoutProperties](./getlayoutproperties/) | Stellt die Eigenschaften des Layouts dar. |
| [Move](./move/) | Verschiebt die Serie nach oben oder unten. |
| [GetPoints](./getpoints/) | Ruft die Sammlung von Punkten in einer Serie in einem Diagramm ab. |
| [GetArea](./getarea/) | Stellt den Hintergrundbereich des Series-Objekts dar. |
| [GetBorder](./getborder/) | Stellt die Grenze eines Series-Objekts dar. |
| [GetName](./getname/) | Liest oder setzt den Namen der Datenserie. |
| [SetName](./setname/) | Liest oder setzt den Namen der Datenserie. |
| [GetDisplayName](./getdisplayname/) | Liest den Namen der Serie, der im Diagramm angezeigt wird. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Liest die Anzahl der Datenwerte. |
| [IsVerticalValues](./isverticalvalues/) | Gibt an, ob die Datenquelle vertikal ist. |
| [GetValues](./getvalues/) | Stellt die Y-Werte dieser Diagrammserie dar. |
| [SetValues](./setvalues/) | Stellt die Y-Werte dieser Diagrammserie dar. |
| [GetPointValues](./getpointvalues/) | Liest die tatsächlichen Werte, die verwendet werden, um jeden Punkt dieser Serie im Diagramm zu plotten. |
| [GetCategoryValues](./getcategoryvalues/) | Liest die tatsächlichen Kategorienwerte, die verwendet werden, um jeden Punkt dieser Serie im Diagramm zu plotten. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Stellt den Formatcode der Werte-NumberList dar. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Stellt den Formatcode der Werte-NumberList dar. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | Stellt den Formatcode der NumberList der X‑Werte dar. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | Stellt den Formatcode der NumberList der X‑Werte dar. |
| [GetXValues](./getxvalues/) | Stellt die X‑Werte dieser Diagrammserie dar. |
| [SetXValues](./setxvalues/) | Stellt die X‑Werte dieser Diagrammserie dar. |
| [GetBubbleSizes](./getbubblesizes/) | Liest oder legt die Bubble‑Größenwerte der Diagrammserie fest. |
| [SetBubbleSizes](./setbubblesizes/) | Liest oder legt die Bubble‑Größenwerte der Diagrammserie fest. |
| [GetTrendLines](./gettrendlines/) | Gibt alle Trendlinien dieser Serie zurück. |
| [GetSmooth](./getsmooth/) | Stellt die Kurvenglättung dar. Wahr, wenn die Kurvenglättung für das Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien. |
| [SetSmooth](./setsmooth/) | Stellt die Kurvenglättung dar. Wahr, wenn die Kurvenglättung für das Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien. |
| [GetShadow](./getshadow/) | Wahr, wenn die Serie einen Schatten hat. |
| [SetShadow](./setshadow/) | Wahr, wenn die Serie einen Schatten hat. |
| [GetHas3DEffect](./gethas3deffect/) | Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat. |
| [SetHas3DEffect](./sethas3deffect/) | Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat. |
| [GetBar3DShapeType](./getbar3dshapetype/) | Liest oder legt den 3D‑Formtyp fest, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird. |
| [SetBar3DShapeType](./setbar3dshapetype/) | Liest oder legt den 3D‑Formtyp fest, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird. |
| [GetDataLabels](./getdatalabels/) | Stellt das DataLabels‑Objekt für die angegebene ASeries dar. |
| [GetType](./gettype/) | Liest oder legt den Typ einer Datenserie fest. |
| [SetType](./settype/) | Liest oder legt den Typ einer Datenserie fest. |
| [GetMarker](./getmarker/) | Liest den Marker</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Gibt an, ob diese Serie auf der zweiten Werteachse dargestellt wird. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Gibt an, ob diese Serie auf der zweiten Werteachse dargestellt wird. |
| [GetXErrorBar](./getxerrorbar/) | Stellt die Fehlerbalken in X‑Richtung der Serie dar. |
| [GetYErrorBar](./getyerrorbar/) | Stellt die Fehlerbalken in Y‑Richtung der Serie dar. |
| [GetHasHiLoLines](./gethashilolines/) | Wahr, wenn das Liniendiagramm Hoch‑Niedrig‑Linien hat. Gilt nur für Liniendiagramme. |
| [SetHasHiLoLines](./sethashilolines/) | Wahr, wenn das Liniendiagramm Hoch‑Niedrig‑Linien hat. Gilt nur für Liniendiagramme. |
| [GetHiLoLines](./gethilolines/) | Gibt ein HiLoLines‑Objekt zurück, das die Hoch‑Niedrig‑Linien für eine Serie in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [GetHasSeriesLines](./gethasserieslines/) | Wahr, wenn ein gestapeltes Säulen‑ oder Balkendiagramm Serienlinien hat oder wenn ein Pie‑of‑Pie‑Diagramm bzw. Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulen‑ und Balkendiagramme, Pie‑of‑Pie‑ und Bar‑of‑Pie‑Diagramme. |
| [SetHasSeriesLines](./sethasserieslines/) | Wahr, wenn ein gestapeltes Säulen‑ oder Balkendiagramm Serienlinien hat oder wenn ein Pie‑of‑Pie‑Diagramm bzw. Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulen‑ und Balkendiagramme, Pie‑of‑Pie‑ und Bar‑of‑Pie‑Diagramme. |
| [GetSeriesLines](./getserieslines/) | Gibt ein SeriesLines‑Objekt zurück, das die Serienlinien für ein gestapeltes Balken‑ oder Säulendiagramm darstellt. Gilt nur für gestapelte Balken‑ und Säulendiagramme. |
| [GetHasDropLines](./gethasdroplines/) | Wahr, wenn das Diagramm Falllinien hat. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [SetHasDropLines](./sethasdroplines/) | Wahr, wenn das Diagramm Falllinien hat. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [GetDropLines](./getdroplines/) | Gibt ein Line‑Objekt zurück, das die Falllinien für eine Serie im Liniendiagramm oder Flächendiagramm darstellt. Gilt nur für Liniendiagramme oder Flächendiagramme. |
| [GetHasUpDownBars](./gethasupdownbars/) | Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. Gilt nur für Liniendiagramme. |
| [SetHasUpDownBars](./sethasupdownbars/) | Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. Gilt nur für Liniendiagramme. |
| [GetUpBars](./getupbars/) | Gibt ein DropBars‑Objekt zurück, das die Auf‑Balken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [GetDownBars](./getdownbars/) | Gibt ein DropBars‑Objekt zurück, das die Ab‑Balken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme. |
| [IsColorVaried](./iscolorvaried/) | Stellt dar, ob die Farbe der Punkte variiert. Das Diagramm muss nur eine Serie enthalten oder ein Kreisdiagramm sein. |
| [SetIsColorVaried](./setiscolorvaried/) | Stellt dar, ob die Farbe der Punkte variiert. Das Diagramm muss nur eine Serie enthalten oder ein Kreisdiagramm sein. |
| [GetGapWidth](./getgapwidth/) | Ruft den Abstand zwischen Balken‑ oder Säulen‑Clustern ab oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [SetGapWidth](./setgapwidth/) | Ruft den Abstand zwischen Balken‑ oder Säulen‑Clustern ab oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Eigenschaft muss zwischen 0 und 500 liegen. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | Liest oder legt den Winkel des ersten Kuchen‑ oder Donut‑Segments in Grad fest (im Uhrzeigersinn von der Vertikalen aus). Gilt nur für Kuchen‑, 3‑D‑Kuchen‑ und Donut‑Diagramme, mit Werten von 0 bis 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | Liest oder legt den Winkel des ersten Kuchen‑ oder Donut‑Segments in Grad fest (im Uhrzeigersinn von der Vertikalen aus). Gilt nur für Kuchen‑, 3‑D‑Kuchen‑ und Donut‑Diagramme, mit Werten von 0 bis 360. |
| [GetOverlap](./getoverlap/) | Gibt an, wie Balken und Säulen positioniert werden.Kann ein Wert zwischen -100 und 100 sein.Gilt nur für 2‑D‑Balken- und 2‑D‑Säulendiagramme. |
| [SetOverlap](./setoverlap/) | Gibt an, wie Balken und Säulen positioniert werden.Kann ein Wert zwischen -100 und 100 sein.Gilt nur für 2‑D‑Balken- und 2‑D‑Säulendiagramme. |
| [GetSecondPlotSize](./getsecondplotsize/) | Gibt die Größe des sekundären Abschnitts eines Kreis‑in‑Kreis‑Diagramms oder eines Balken‑in‑Kreis‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kreises.Kann ein Wert von 5 bis 200 sein. |
| [SetSecondPlotSize](./setsecondplotsize/) | Gibt die Größe des sekundären Abschnitts eines Kreis‑in‑Kreis‑Diagramms oder eines Balken‑in‑Kreis‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kreises.Kann ein Wert von 5 bis 200 sein. |
| [GetSplitType](./getsplittype/) | Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [SetSplitType](./setsplittype/) | Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [GetSplitValue](./getsplitvalue/) | Gibt einen Wert zurück oder legt ihn fest, der verwendet werden soll, um zu bestimmen, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [SetSplitValue](./setsplitvalue/) | Gibt einen Wert zurück oder legt ihn fest, der verwendet werden soll, um zu bestimmen, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen. |
| [IsAutoSplit](./isautosplit/) | Gibt an, ob der Schwellenwert automatisch ist. |
| [GetBubbleScale](./getbubblescale/) | Liest oder legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest.Kann ein ganzzahliger Wert von 0 (null) bis 300 sein, entsprechend einem Prozentsatz der Standardgröße.Gilt nur für Blasendiagramme. |
| [SetBubbleScale](./setbubblescale/) | Liest oder legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest.Kann ein ganzzahliger Wert von 0 (null) bis 300 sein, entsprechend einem Prozentsatz der Standardgröße.Gilt nur für Blasendiagramme. |
| [GetSizeRepresents](./getsizerepresents/) | Liest oder legt fest, was die Blasengröße in einem Blasendiagramm darstellt. |
| [SetSizeRepresents](./setsizerepresents/) | Liest oder legt fest, was die Blasengröße in einem Blasendiagramm darstellt. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Nur für Blasendiagramme gültig. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Nur für Blasendiagramme gültig. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Gibt die Größe des Lochs in einer Donut‑Diagrammgruppe zurück oder legt sie fest.Die Lochgröße wird als Prozentsatz der Diagrammgröße angegeben, zwischen 10 und 90 Prozent. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Gibt die Größe des Lochs in einer Donut‑Diagrammgruppe zurück oder legt sie fest.Die Lochgröße wird als Prozentsatz der Diagrammgröße angegeben, zwischen 10 und 90 Prozent. |
| [GetExplosion](./getexplosion/) | Der Abstand eines offenen Kuchensegments vom Mittelpunkt des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [SetExplosion](./setexplosion/) | Der Abstand eines offenen Kuchensegments vom Mittelpunkt des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | True, wenn ein Radar‑Diagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radar‑Diagramme. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | True, wenn ein Radar‑Diagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radar‑Diagramme. |
| [GetHasLeaderLines](./gethasleaderlines/) | True, wenn die Serie Führungslinien hat. |
| [SetHasLeaderLines](./sethasleaderlines/) | True, wenn die Serie Führungslinien hat. |
| [GetLeaderLines](./getleaderlines/) | Stellt Führungslinien in einem Diagramm dar. Führungslinien verbinden Datenbeschriftungen mit Datenpunkten.Dieses Objekt ist keine Sammlung; es gibt kein Objekt, das eine einzelne Führungslinie darstellt. |
| [GetLegendEntry](./getlegendentry/) | Liest den Legendeintrag gemäß dieser Serie. |
| [GetShapeProperties](./getshapeproperties/) | Liest das ShapePropertyCollection‑Objekt, das die visuellen Formeigenschaften der Serie enthält. |
