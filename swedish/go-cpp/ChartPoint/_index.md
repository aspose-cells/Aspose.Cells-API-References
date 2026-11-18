---
title: "ChartPoint-klass"
linktitle: "ChartPoint"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ChartPoint-klass. Inkapslar objektet som representerar chartpoint i Go."
type: docs
weight: 200
url: /sv/go-cpp/chartpoint/
---

## ChartPoint class

Representerar en enskild punkt i en serie i ett diagram.

```go

type ChartPoint struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetExplosion](./getexplosion/) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [SetExplosion](./setexplosion/) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [GetShadow](./getshadow/) | Sant om chartpoint har en skugga. |
| [SetShadow](./setshadow/) | Sant om chartpoint har en skugga. |
| [GetBorder](./getborder/) | Hämtar Line</see>. |
| [GetArea](./getarea/) | Hämtar Area</see>. |
| [GetMarker](./getmarker/) | Hämtar Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Returnerar ett DataLabels-objekt som representerar datamärket som är associerat med denna diagrampunkt. |
| [Get_YValue](./get_yvalue/) | Hämtar eller anger Y‑värdet för diagrampunkten. |
| [SetYValue](./setyvalue/) | Hämtar eller anger Y‑värdet för diagrampunkten. |
| [GetYValueType](./getyvaluetype/) | Hämtar Y‑värdestypen för diagrampunkten. |
| [GetXValue](./getxvalue/) | Hämtar eller anger X‑värdet för diagrampunkten. |
| [SetXValue](./setxvalue/) | Hämtar eller anger X‑värdet för diagrampunkten. |
| [GetXValueType](./getxvaluetype/) | Hämtar X‑värdestypen för diagrampunkten. |
| [GetShapeProperties](./getshapeproperties/) | Hämtar ShapePropertyCollection-objektet som innehåller de visuella formegenskaperna för ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Hämtar eller anger ett värde som indikerar om denna datapunkt är i den andra delen eller stapeln i ett pie‑ eller bar‑diagram. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Hämtar eller anger ett värde som indikerar om denna datapunkt är i den andra delen eller stapeln i ett pie‑ eller bar‑diagram. |
| [GetShapeX](./getshapex/) | Hämtar x‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets bredd efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeY](./getshapey/) | Hämtar y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | Hämtar bredden i enheter av 1/4000 av diagrammets bredd efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | Hämtar höjden i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Hämtar x‑koordinaten för det övre vänstra hörnet i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Hämtar y‑koordinaten för det övre vänstra hörnet i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Hämtar bredden i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Hämtar höjden i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Hämtar kantens bredd i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Hämtar radien för bubbla, paj eller donut i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Hämtar den inre radien för en donut-slice i pixelenheter efter anrop av metoden Chart.Calculate(). Gäller för donut-diagram. |
| [GetStartAngle](./getstartangle/) | Hämtar startvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter anrop av metoden Chart.Calculate(). Gäller för paj-diagram. |
| [GetEndAngle](./getendangle/) | Hämtar slutvinkeln för pajsektionen, mätt i grader medurs från x-axeln efter anrop av metoden Chart.Calculate(). Gäller för paj-diagram. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Hämtar x-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för paj- och donut-diagram. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Hämtar y-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för paj- och donut-diagram. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Hämtar x-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för paj- och donut-diagram. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Hämtar y-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för paj- och donut-diagram. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Hämtar x-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för donut-diagrammet. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Hämtar y-koordinaten för startpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för donut-diagrammet. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Hämtar x-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för donut-diagram. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Hämtar y-koordinaten för slutpunkten för pajsektionen efter anrop av metoden Chart.Calculate(). Gäller för donut-diagrammet. |
| [GetTopPointCount](./gettoppointcount/) | Hämtar antalet toppunkter efter anrop av metoden Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Hämtar x-koordinaten för toppunkten på formen efter anrop av metoden Chart.Calculate(). Gäller 3D-diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D. |
| [GetTopPointYPx](./gettoppointypx/) | Hämtar y-koordinaten för toppunkten på formen efter anrop av metoden Chart.Calculate(). Gäller 3D-diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid och Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Hämtar antalet bottenpunkter efter anrop av metoden Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Hämtar x-koordinaten för bottenpunkten på formen efter anrop av metoden Chart.Calculate(). Gäller för 3D-diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetBottomPointYPx](./getbottompointypx/) | Hämtar y-koordinaten för bottenpunkten på formen efter anrop av metoden Chart.Calculate(). Gäller för 3D-diagram: Column3D, Bar3D, Cone, Cylinder, Pyramid. |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Hämtar antalet punkter på kategoraxeln efter anrop av metoden Chart.Calculate(). Gäller endast för area-diagram. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Hämtar x-koordinaten för punkten på kategoraxeln efter anrop av metoden Chart.Calculate(). Gäller endast för area-diagram. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Hämtar y-koordinaten för punkten på kategoraxeln efter anrop av metoden Chart.Calculate(). Gäller endast för area-diagram. |
