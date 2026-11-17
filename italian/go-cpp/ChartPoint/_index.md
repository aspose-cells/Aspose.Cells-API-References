---
title: "Classe ChartPoint"
linktitle: "ChartPoint"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ChartPoint. Incapsula l'oggetto che rappresenta chartpoint in Go."
type: docs
weight: 200
url: /it/go-cpp/chartpoint/
---

## ChartPoint class

Rappresenta un singolo punto in una serie in un grafico.

```go

type ChartPoint struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetExplosion](./getexplosion/) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [SetExplosion](./setexplosion/) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [GetShadow](./getshadow/) | Vero se il chartpoint ha un'ombra. |
| [SetShadow](./setshadow/) | Vero se il chartpoint ha un'ombra. |
| [GetBorder](./getborder/) | Ottiene il Line</see>. |
| [GetArea](./getarea/) | Ottiene l'Area</see>. |
| [GetMarker](./getmarker/) | Ottiene il Marker</see>. |
| [GetDataLabels](./getdatalabels/) | Restituisce un oggetto DataLabels che rappresenta l'etichetta dati associata a questo punto del grafico. |
| [Get_YValue](./get_yvalue/) | Ottiene o imposta il valore Y del punto del grafico. |
| [SetYValue](./setyvalue/) | Ottiene o imposta il valore Y del punto del grafico. |
| [GetYValueType](./getyvaluetype/) | Ottiene il tipo di valore Y del punto del grafico. |
| [GetXValue](./getxvalue/) | Ottiene o imposta il valore X del punto del grafico. |
| [SetXValue](./setxvalue/) | Ottiene o imposta il valore X del punto del grafico. |
| [GetXValueType](./getxvaluetype/) | Ottiene il tipo di valore X del punto del grafico. |
| [GetShapeProperties](./getshapeproperties/) | Ottiene l'oggetto ShapePropertyCollection che contiene le proprietà visive della forma del ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | Ottiene o imposta un valore che indica se questo punto dati si trova nella seconda torta o barra su una torta di torta o barra di grafico a torta. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | Ottiene o imposta un valore che indica se questo punto dati si trova nella seconda torta o barra su una torta di torta o barra di grafico a torta. |
| [GetShapeX](./getshapex/) | Ottiene la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeY](./getshapey/) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | Ottiene la larghezza in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | Ottiene l'altezza in unità di 1/4000 dell'altezza del grafico dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | Ottiene la coordinata x dell'angolo in alto a sinistra in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | Ottiene la coordinata y dell'angolo in alto a sinistra in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | Ottiene la larghezza in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | Ottiene l'altezza in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | Ottiene la larghezza del bordo in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | Ottiene il raggio di bolla, torta o ciambella in pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | Ottiene il raggio interno della fetta di ciambella in pixel dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Doughnut. |
| [GetStartAngle](./getstartangle/) | Ottiene l'angolo iniziale per la sezione della torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Pie. |
| [GetEndAngle](./getendangle/) | Ottiene l'angolo finale per la sezione della torta, misurato in gradi in senso orario dall'asse x dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Pie. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | Ottiene la coordinata x del punto iniziale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici Pie e Doughnut. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | Ottiene la coordinata y del punto iniziale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici Pie e Doughnut. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | Ottiene la coordinata x del punto finale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici Pie e Doughnut. |
| [GetArcEndPointYPx](./getarcendpointypx/) | Ottiene la coordinata y del punto finale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici Pie e Doughnut. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | Ottiene la coordinata x del punto iniziale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Doughnut. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | Ottiene la coordinata y del punto iniziale per la sezione della torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico Doughnut. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | Ottiene la coordinata x del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate().Applica ai grafici a ciambella. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | Ottiene la coordinata y del punto finale della sezione a torta dopo aver chiamato il metodo Chart.Calculate().Applica al grafico a ciambella. |
| [GetTopPointCount](./gettoppointcount/) | Ottiene il numero di punti superiori dopo aver chiamato il metodo Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | Ottiene la coordinata x del punto superiore della forma dopo aver chiamato il metodo Chart.Calculate().Applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D |
| [GetTopPointYPx](./gettoppointypx/) | Ottiene la coordinata y del punto superiore della forma dopo aver chiamato il metodo Chart.Calculate().Applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | Ottiene il numero di punti inferiori dopo aver chiamato il metodo Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | Ottiene la coordinata x del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate().Applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetBottomPointYPx](./getbottompointypx/) | Ottiene la coordinata y del punto inferiore della forma dopo aver chiamato il metodo Chart.Calculate().Applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | Ottiene il numero dei punti sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate().Si applica solo ai grafici ad area. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | Ottiene la coordinata x del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate().Si applica solo al grafico ad area. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | Ottiene la coordinata y del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate().Si applica solo al grafico ad area. |
