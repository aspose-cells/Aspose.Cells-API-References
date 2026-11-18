---
title: "DataBar-klass"
linktitle: "DataBar"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DataBar-klass. Inkapslar objektet som representerar databar i Go."
type: docs
weight: 200
url: /sv/go-cpp/databar/
---

## DataBar class

Beskriv DataBar‑villkorsformateringsregeln. Denna villkorsformateringsregel visar en graderad datastapel i cellområdet.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Hämtar färgen på axeln för celler med villkorsstyrd formatering som datastaplar. |
| [SetAxisColor](./setaxiscolor/) | Hämtar färgen på axeln för celler med villkorsstyrd formatering som datastaplar. |
| [GetAxisPosition](./getaxisposition/) | Hämtar eller anger positionen för axeln på datastaplarna som specificeras av en villkorsstyrd formateringsregel. |
| [SetAxisPosition](./setaxisposition/) | Hämtar eller anger positionen för axeln på datastaplarna som specificeras av en villkorsstyrd formateringsregel. |
| [GetBarFillType](./getbarfilltype/) | Hämtar eller anger hur en datastapel fylls med färg. |
| [SetBarFillType](./setbarfilltype/) | Hämtar eller anger hur en datastapel fylls med färg. |
| [GetDirection](./getdirection/) | Hämtar eller anger riktningen som datastapeln visas i. |
| [SetDirection](./setdirection/) | Hämtar eller anger riktningen som datastapeln visas i. |
| [GetBarBorder](./getbarborder/) | Hämtar ett objekt som specificerar kanten på en datastapel. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Hämtar NegativeBarFormat-objektet som är associerat med en villkorsstyrd formateringsregel för en datastapel. |
| [GetMinCfvo](./getmincfvo/) | Hämta eller ange detta DataBars minvärdesobjekt. Kan inte sätta null eller CFValueObject med typ FormatConditionValueType.Max till det. |
| [GetMaxCfvo](./getmaxcfvo/) | Hämta eller ange detta DataBars maxvärdesobjekt. Kan inte sätta null eller CFValueObject med typ FormatConditionValueType.Min till det. |
| [GetColor](./getcolor/) | Hämta eller ange detta DataBars färg. |
| [SetColor](./setcolor/) | Hämta eller ange detta DataBars färg. |
| [GetMinLength](./getminlength/) | Representerar minsta längden på datastapeln. |
| [SetMinLength](./setminlength/) | Representerar minsta längden på datastapeln. |
| [GetMaxLength](./getmaxlength/) | Representerar största längden på datastapeln. |
| [SetMaxLength](./setmaxlength/) | Representerar största längden på datastapeln. |
| [GetShowValue](./getshowvalue/) | Hämta eller ange flaggan som indikerar om värdena i cellerna som denna datastapel tillämpas på ska visas. Standardvärdet är true. |
| [SetShowValue](./setshowvalue/) | Hämta eller ange flaggan som indikerar om värdena i cellerna som denna datastapel tillämpas på ska visas. Standardvärdet är true. |
| [ToImage](./toimage/) | Rendera datastapel i cell till bildbytearray. |
