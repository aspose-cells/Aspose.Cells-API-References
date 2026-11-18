---
title: "Walls-klass"
linktitle: "Walls"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Walls-klass. Inkapslar objektet som representerar väggar i Go."
type: docs
weight: 200
url: /sv/go-cpp/walls/
---

## Walls class

Inkapslar objektet som representerar väggarna i ett 3‑D-diagram.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewWalls](./newwalls/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetCenterX](./getcenterx/) | Hämtar x-koordinaten för det vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [GetCenterY](./getcentery/) | Hämtar y-koordinaten för det vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate(). |
| [GetWidth](./getwidth/) | Hämtar bredden från vänster till höger i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [GetDepth](./getdepth/) | Hämtar djupet fram till bak i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [GetHeight](./getheight/) | Hämtar höjden från topp till botten i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate(). |
| [GetCenterXPx](./getcenterxpx/) | Hämtar x-koordinaten för det nedre‑vänstra hörnet av väggens centrum i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetCenterYPx](./getcenterypx/) | Hämtar y-koordinaten för det vänster‑nedre hörnet av väggens centrum i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetWidthPx](./getwidthpx/) | Hämtar bredden från vänster till höger i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetDepthPx](./getdepthpx/) | Hämtar djupet fram till bak i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetHeightPx](./getheightpx/) | Hämtar höjden från topp till botten i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [GetCubePointCount](./getcubepointcount/) | Hämtar antalet kubpunkter efter anrop av metoden Chart.Calculate(). |
| [GetCubePointXPx](./getcubepointxpx/) | Hämtar x-koordinaten för apex‑punkten i väggkuben efter anrop av metoden Chart.Calculate(). Antalet apex‑punkter i väggkuben är åtta. |
| [GetCubePointYPx](./getcubepointypx/) | Hämtar y-koordinaten för apex‑punkten i väggkuben efter anrop av metoden Chart.Calculate(). Antalet apex‑punkter i väggkuben är åtta. |
| [GetBackgroundColor](./getbackgroundcolor/) | Hämtar eller anger bakgrund Color för Area. |
| [SetBackgroundColor](./setbackgroundcolor/) | Hämtar eller anger bakgrund Color för Area. |
| [GetForegroundColor](./getforegroundcolor/) | Hämtar eller anger foreground Color. |
| [SetForegroundColor](./setforegroundcolor/) | Hämtar eller anger foreground Color. |
| [GetFormatting](./getformatting/) | Representerar formateringen av området. |
| [SetFormatting](./setformatting/) | Representerar formateringen av området. |
| [GetInvertIfNegative](./getinvertifnegative/) | Om egenskapen är sann och värdet för chart point är ett negativt tal, kommer foreground color och background color att bytas. |
| [SetInvertIfNegative](./setinvertifnegative/) | Om egenskapen är sann och värdet för chart point är ett negativt tal, kommer foreground color och background color att bytas. |
| [GetFillFormat](./getfillformat/) | Representerar ett FillFormat-objekt som innehåller fyllningsformaterings-egenskaper för det angivna diagrammet eller formen. |
| [GetTransparency](./gettransparency/) | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) till 1.0 (klar). |
| [SetTransparency](./settransparency/) | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) till 1.0 (klar). |
| [GetBorder](./getborder/) | Hämtar eller anger border Line. |
| [SetBorder](./setborder/) | Hämtar eller anger border Line. |
