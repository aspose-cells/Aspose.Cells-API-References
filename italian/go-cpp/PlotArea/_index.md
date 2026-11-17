---
title: "PlotArea Class"
linktitle: "PlotArea"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PlotArea class. Incapsula l'oggetto che rappresenta plotarea in Go."
type: docs
weight: 200
url: /it/go-cpp/plotarea/
---

## PlotArea class

Incapsula l'oggetto che rappresenta l'area di tracciamento in un grafico.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPlotArea](./newplotarea/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra del riquadro di delimitazione dell'area del grafico come rapporto dell'area del diagramma. |
| [SetXRatioToChart](./setxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra del riquadro di delimitazione dell'area del grafico come rapporto dell'area del diagramma. |
| [GetYRatioToChart](./getyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo superiore dell'area del grafico del riquadro di delimitazione come rapporto dell'area del diagramma. |
| [SetYRatioToChart](./setyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo superiore dell'area del grafico del riquadro di delimitazione come rapporto dell'area del diagramma. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Ottiene o imposta l'altezza del riquadro di delimitazione dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Ottiene o imposta l'altezza del riquadro di delimitazione dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Ottiene o imposta la larghezza del riquadro di delimitazione dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Ottiene o imposta la larghezza del riquadro di delimitazione dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | Ottiene o ottiene la coordinata x dell'angolo superiore dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | Ottiene o ottiene la coordinata x dell'angolo superiore dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | Ottiene o ottiene la coordinata x dell'angolo superiore dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | Ottiene o ottiene la coordinata x dell'angolo superiore dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | Ottiene o imposta l'altezza dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | Ottiene o imposta l'altezza dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | Ottiene o imposta la larghezza dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | Ottiene o imposta la larghezza dell'area del grafico in unità del rapporto dell'area del diagramma. |
| [SetPositionAuto](./setpositionauto/) | Imposta la posizione dell'area del grafico su automatico |
| [IsAutomaticSize](./isautomaticsize/) | Indica se l'area del grafico è dimensionata automaticamente. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indica se l'area del grafico è dimensionata automaticamente. |
| [IsInnerMode](./isinnermode/) | Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, dei segni di graduazione e delle etichette degli assi. |
| [SetIsInnerMode](./setisinnermode/) | Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, dei segni di graduazione e delle etichette degli assi. |
| [GetShadow](./getshadow/) | True se il frame ha un'ombra. |
| [SetShadow](./setshadow/) | True se il frame ha un'ombra. |
| [GetShapeProperties](./getshapeproperties/) | Ottiene l'oggetto ShapeProperties. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Rappresenta x della posizione predefinita in unità di Fraction dell'area del diagramma. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Rappresenta y della posizione predefinita in unità della frazione dell'area del diagramma. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Rappresenta la larghezza della posizione predefinita in unità di Fraction dell'area del diagramma. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del diagramma. |
| [GetBorder](./getborder/) | Ottiene il Line</see>. |
| [GetArea](./getarea/) | Ottiene l'Area</see>. |
| [GetTextOptions](./gettextoptions/) | Ottiene e imposta le opzioni del testo. |
| [GetFont](./getfont/) | Ottiene un oggetto Font dell'oggetto ChartFrame specificato. |
| [GetAutoScaleFont](./getautoscalefont/) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True. |
| [SetAutoScaleFont](./setautoscalefont/) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True. |
| [GetXPixel](./getxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [SetXPixel](./setxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [GetYPixel](./getypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [SetYPixel](./setypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [GetWidthPixel](./getwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [GetHeightPixel](./getheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
| [SetHeightPixel](./setheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
