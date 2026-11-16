---
title: "ChartPoint Klasse"
linktitle: "ChartPoint"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ChartPoint Klasse. Kapselt das Objekt, das ChartPoint in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/chartpoint/
---

## ChartPoint class

Stellt einen einzelnen Punkt in einer Serie in einem Diagramm dar.

```go

type ChartPoint struct  {
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
| [GetExplosion](./getexplosion/) | Der Abstand eines offenen Kuchensegments vom Mittelpunkt des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [SetExplosion](./setexplosion/) | Der Abstand eines offenen Kuchensegments vom Mittelpunkt des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [GetShadow](./getshadow/) | Wahr, wenn der ChartPoint einen Schatten hat. |
| [SetShadow](./setshadow/) | Wahr, wenn der ChartPoint einen Schatten hat. |
| [GetBorder](./getborder/) | Liest die Line</see>. |
| [GetArea](./getarea/) | Liest die Area</see>. |
| [GetMarker](./getmarker/) | Liest den Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Gibt ein DataLabels-Objekt zurück, das das mit diesem Diagrammpunkt verbundene Datenbeschriftungsobjekt darstellt. |
| [Get_YValue](./get_yvalue/) | Liest oder setzt den Y-Wert des Diagrammpunkts. |
| [SetYValue](./setyvalue/) | Liest oder setzt den Y-Wert des Diagrammpunkts. |
| [GetYValueType](./getyvaluetype/) | Liest den Y-Werttyp des Diagrammpunkts. |
| [GetXValue](./getxvalue/) | Liest oder setzt den X-Wert des Diagrammpunkts. |
| [SetXValue](./setxvalue/) | Liest oder setzt den X-Wert des Diagrammpunkts. |
| [GetXValueType](./getxvaluetype/) | Liest den X-Werttyp des Diagrammpunkts. |
| [GetShapeProperties](./getshapeproperties/) | Liest das ShapePropertyCollection-Objekt, das die visuellen Formeigenschaften des ChartPoint enthält. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Liest oder setzt einen Wert, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kreis- bzw. Balkendiagramms liegt. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Liest oder setzt einen Wert, der angibt, ob dieser Datenpunkt im zweiten Kuchen oder Balken eines Kreis- bzw. Balkendiagramms liegt. |
| [GetShapeX](./getshapex/) | Liest die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammbreite, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetShapeY](./getshapey/) | Liest die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 der Diagrammhöhe, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetShapeWidth](./getshapewidth/) | Liest die Breite in Einheiten von 1/4000 der Diagrammbreite, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [GetShapeHeight](./getshapeheight/) | Ermittelt die Höhe in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Ermittelt die x‑Koordinate der oberen linken Ecke in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Ermittelt die y‑Koordinate der oberen linken Ecke in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Ermittelt die Breite in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Ermittelt die Höhe in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Ermittelt die Breite des Rahmens in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Ermittelt den Radius von Bubble-, Pie- oder Doughnut-Diagrammen in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Ermittelt den inneren Radius eines Doughnut‑Segments in Pixeln nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramm. |
| [GetStartAngle](./getstartangle/) | Ermittelt den Startwinkel für das Pie‑Segment, gemessen in Grad im Uhrzeigersinn von der x‑Achse nach Aufruf der Methode Chart.Calculate(). Gilt für Pie-Diagramme. |
| [GetEndAngle](./getendangle/) | Ermittelt den Endwinkel für das Pie‑Segment, gemessen in Grad im Uhrzeigersinn von der x‑Achse nach Aufruf der Methode Chart.Calculate(). Gilt für Pie-Diagramme. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Ermittelt die x‑Koordinate des Startpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für Pie‑ und Doughnut-Diagramme. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Ermittelt die y‑Koordinate des Startpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für Pie‑ und Doughnut-Diagramme. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Ermittelt die x‑Koordinate des Endpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für Pie‑ und Doughnut-Diagramme. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Ermittelt die y‑Koordinate des Endpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für Pie‑ und Doughnut-Diagramme. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Ermittelt die x‑Koordinate des Startpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für das Doughnut-Diagramm. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Ermittelt die y‑Koordinate des Startpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für das Doughnut-Diagramm. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Ermittelt die x‑Koordinate des Endpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für Doughnut-Diagramme. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Ermittelt die y‑Koordinate des Endpunkts des Pie‑Segments nach Aufruf der Methode Chart.Calculate(). Gilt für das Doughnut-Diagramm. |
| [GetTopPointCount](./gettoppointcount/) | Ermittelt die Anzahl der oberen Punkte nach Aufruf der Methode Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Ermittelt die x‑Koordinate des oberen Punkts der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D. |
| [GetTopPointYPx](./gettoppointypx/) | Ermittelt die y‑Koordinate des oberen Punkts der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid und Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Ermittelt die Anzahl der unteren Punkte nach Aufruf der Methode Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Ermittelt die x‑Koordinate des unteren Punkts der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetBottomPointYPx](./getbottompointypx/) | Ermittelt die y‑Koordinate des unteren Punkts der Form nach Aufruf der Methode Chart.Calculate(). Gilt für 3D-Diagramme: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Ermittelt die Anzahl der Punkte auf der Kategorienachse nach Aufruf der Chart.Calculate()-Methode.Gilt nur für Flächendiagramme. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Ermittelt die x-Koordinate des Punktes auf der Kategorienachse nach Aufruf der Chart.Calculate()-Methode.Gilt nur für Flächendiagramme. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Ermittelt die y-Koordinate des Punktes auf der Kategorienachse nach Aufruf der Chart.Calculate()-Methode.Gilt nur für Flächendiagramme. |
