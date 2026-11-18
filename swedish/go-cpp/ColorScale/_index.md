---
title: "ColorScale-klass"
linktitle: "ColorScale"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ColorScale-klass. Inkapslar objektet som representerar colorscale i Go."
type: docs
weight: 200
url: /sv/go-cpp/colorscale/
---

## ColorScale class

Beskriv ColorScale‑villkorsformateringsregeln. Denna villkorsformateringsregel skapar en graderad färgskala på cellerna.

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | Anger om villkorsformatering är en 3-färgs skala. |
| [SetIs3ColorScale](./setis3colorscale/) | Anger om villkorsformatering är en 3-färgs skala. |
| [GetMinCfvo](./getmincfvo/) | Hämta eller ange detta ColorScale:s minvärdesobjekt.Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Max till det. |
| [GetMidCfvo](./getmidcfvo/) | Hämta eller ange detta ColorScale:s mittvärdesobjekt.Kan inte sätta CFValueObject med typen FormatConditionValueType.Max eller FormatConditionValueType.Min till det. |
| [GetMaxCfvo](./getmaxcfvo/) | Hämta eller ange detta ColorScale:s maxvärdesobjekt.Kan inte sätta null eller CFValueObject med typen FormatConditionValueType.Min till det. |
| [GetMinColor](./getmincolor/) | Hämta eller ange gradientfärgen för det minsta värdet i intervallet. |
| [SetMinColor](./setmincolor/) | Hämta eller ange gradientfärgen för det minsta värdet i intervallet. |
| [GetMidColor](./getmidcolor/) | Hämta eller ange gradientfärgen för det mellersta värdet i intervallet. |
| [SetMidColor](./setmidcolor/) | Hämta eller ange gradientfärgen för det mellersta värdet i intervallet. |
| [GetMaxColor](./getmaxcolor/) | Hämta eller ange gradientfärgen för det största värdet i intervallet. |
| [SetMaxColor](./setmaxcolor/) | Hämta eller ange gradientfärgen för det största värdet i intervallet. |
