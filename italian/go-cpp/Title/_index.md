---
title: "Classe Title"
linktitle: "Title"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Title. Incapsula l'oggetto che rappresenta il titolo in Go."
type: docs
weight: 200
url: /it/go-cpp/title/
---

## Title class

Incapsula l'oggetto che rappresenta il titolo del grafico o dell'asse.

```go

type Title struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTitle](./newtitle/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetText](./gettext/) | Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione. |
| [SetText](./settext/) | Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione. |
| [IsVisible](./isvisible/) | Rappresenta se il titolo è visibile. |
| [SetIsVisible](./setisvisible/) | Rappresenta se il titolo è visibile. |
| [GetXRatioToChart](./getxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico.X in pixel = XRatioToChart * Chart.ChartObject.Width; |
| [SetXRatioToChart](./setxratiotochart/) | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico.X in pixel = XRatioToChart * Chart.ChartObject.Width; |
| [GetYRatioToChart](./getyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico.Y in pixel = YRatioToChart * Chart.ChartObject.Width; |
| [SetYRatioToChart](./setyratiotochart/) | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico.Y in pixel = YRatioToChart * Chart.ChartObject.Width; |
| [GetOverLay](./getoverlay/) | Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico. |
| [SetOverLay](./setoverlay/) | Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico. |
| [Characters](./characters/) | Ottiene la formattazione del testo ricco di questo Title. |
| [Characters_Int_Int](./characters_int_int/) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo. |
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
| [IsAutomaticSize](./isautomaticsize/) | Indica se il frame del grafico è dimensionato automaticamente. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Indica se il frame del grafico è dimensionato automaticamente. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Ottiene o imposta la larghezza del frame in unità del rapporto dell'area del grafico. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Ottiene o imposta la larghezza del frame in unità del rapporto dell'area del grafico. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [GetXPixel](./getxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [SetXPixel](./setxpixel/) | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di Pixel. |
| [GetYPixel](./getypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [SetYPixel](./setypixel/) | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di pixel. |
| [GetWidthPixel](./getwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [SetWidthPixel](./setwidthpixel/) | Ottiene o imposta la larghezza del frame in unità di Pixel. |
| [GetHeightPixel](./getheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
| [SetHeightPixel](./setheightpixel/) | Ottiene o imposta l'altezza del frame in unità di pixel. |
| [SetPositionAuto](./setpositionauto/) | Imposta la posizione del frame su automatico |
| [IsDeleted](./isdeleted/) | Indica se questa etichetta dati è eliminata. |
| [SetIsDeleted](./setisdeleted/) | Indica se questa etichetta dati è eliminata. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Ottiene e imposta l'allineamento orizzontale del testo. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Ottiene e imposta l'allineamento orizzontale del testo. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Ottiene o imposta l'allineamento verticale del testo. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Ottiene o imposta l'allineamento verticale del testo. |
| [GetRotationAngle](./getrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [SetRotationAngle](./setrotationangle/) | Rappresenta l'angolo di rotazione del testo. |
| [IsAutomaticRotation](./isautomaticrotation/) | Indica se il testo del grafico è ruotato automaticamente. |
| [GetReadingOrder](./getreadingorder/) | Rappresenta l'ordine di lettura del testo. |
| [SetReadingOrder](./setreadingorder/) | Rappresenta l'ordine di lettura del testo. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo. |
| [IsAutoText](./isautotext/) | Indica che il testo è generato automaticamente. |
| [SetIsAutoText](./setisautotext/) | Indica che il testo è generato automaticamente. |
| [GetLinkedSource](./getlinkedsource/) | Ottiene e imposta un riferimento al foglio di lavoro. |
| [SetLinkedSource](./setlinkedsource/) | Ottiene e imposta un riferimento al foglio di lavoro. |
| [GetDirectionType](./getdirectiontype/) | Ottiene e imposta la direzione del testo. |
| [SetDirectionType](./setdirectiontype/) | Ottiene e imposta la direzione del testo. |
| [IsTextWrapped](./istextwrapped/) | Ottiene o imposta un valore che indica se il testo è a capo. |
| [SetIsTextWrapped](./setistextwrapped/) | Ottiene o imposta un valore che indica se il testo è a capo. |
