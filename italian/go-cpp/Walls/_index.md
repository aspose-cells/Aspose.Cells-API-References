---
title: "Classe Walls"
linktitle: "Walls"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Walls. Incapsula l'oggetto che rappresenta i muri in Go."
type: docs
weight: 200
url: /it/go-cpp/walls/
---

## Walls class

Incapsula l'oggetto che rappresenta le pareti di un grafico 3-D.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewWalls](./newwalls/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetCenterX](./getcenterx/) | Ottiene la coordinata x dell'angolo sinistro-inferiore del centro del Wall in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [GetCenterY](./getcentery/) | Ottiene la coordinata y dell'angolo sinistro-inferiore del centro del Wall in unità di 1/4000 dell'altezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [GetWidth](./getwidth/) | Ottiene la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [GetDepth](./getdepth/) | Ottiene la profondità da fronte a retro in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [GetHeight](./getheight/) | Ottiene l'altezza dall'alto al basso in unità di 1/4000 dell'altezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [GetCenterXPx](./getcenterxpx/) | Ottiene la coordinata x dell'angolo inferiore sinistro del centro del Wall in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [GetCenterYPx](./getcenterypx/) | Ottiene la coordinata y dell'angolo sinistro-inferiore del centro del Wall in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [GetWidthPx](./getwidthpx/) | Ottiene la larghezza da sinistra a destra in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [GetDepthPx](./getdepthpx/) | Ottiene la profondità da fronte a retro in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [GetHeightPx](./getheightpx/) | Ottiene l'altezza dall'alto verso il basso in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [GetCubePointCount](./getcubepointcount/) | Ottiene il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate(). |
| [GetCubePointXPx](./getcubepointxpx/) | Ottiene la coordinata x del punto di apice del cubo delle pareti dopo aver chiamato il metodo Chart.Calculate().Il numero di punti di apice del cubo delle pareti è otto |
| [GetCubePointYPx](./getcubepointypx/) | Ottiene la coordinata y del punto di apice del cubo delle pareti dopo le chiamate al metodo Chart.Calculate().Il numero di punti di apice del cubo delle pareti è otto. |
| [GetBackgroundColor](./getbackgroundcolor/) | Ottiene o imposta il colore di sfondo dell'area. |
| [SetBackgroundColor](./setbackgroundcolor/) | Ottiene o imposta il colore di sfondo dell'area. |
| [GetForegroundColor](./getforegroundcolor/) | Ottiene o imposta il colore di primo piano. |
| [SetForegroundColor](./setforegroundcolor/) | Ottiene o imposta il colore di primo piano. |
| [GetFormatting](./getformatting/) | Rappresenta la formattazione dell'area. |
| [SetFormatting](./setformatting/) | Rappresenta la formattazione dell'area. |
| [GetInvertIfNegative](./getinvertifnegative/) | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. |
| [SetInvertIfNegative](./setinvertifnegative/) | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. |
| [GetFillFormat](./getfillformat/) | Rappresenta un oggetto FillFormat che contiene le proprietà di formattazione del riempimento per il grafico o la forma specificati. |
| [GetTransparency](./gettransparency/) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [SetTransparency](./settransparency/) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [GetBorder](./getborder/) | Ottiene o imposta la linea del bordo. |
| [SetBorder](./setborder/) | Ottiene o imposta la linea del bordo. |
