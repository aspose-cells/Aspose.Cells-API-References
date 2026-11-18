---
title: "IconSet klass"
linktitle: "IconSet"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "IconSet klass. Inkapslar objektet som representerar iconset i Go."
type: docs
weight: 200
url: /sv/go-cpp/iconset/
---

## IconSet class

Beskriv IconSet‑villkorsformateringsregeln. Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden.

```go

type IconSet struct  {
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
| [GetCfIcons](./getcficons/) | Hämta theConditionalFormattingIcon från samlingen |
| [GetCfvos](./getcfvos/) | Hämta CFValueObjects-instansen. |
| [GetType](./gettype/) | Hämta eller ange ikonsättets typ för visning. Att ange typen kommer automatiskt att kontrollera om det aktuella Cfvos‑antalet stämmer överens med den nya typen. Om det inte stämmer, kommer gamla Cfvos att rensas och standard‑Cfvos att läggas till. |
| [SetType](./settype/) | Hämta eller ange ikonsättets typ för visning. Att ange typen kommer automatiskt att kontrollera om det aktuella Cfvos‑antalet stämmer överens med den nya typen. Om det inte stämmer, kommer gamla Cfvos att rensas och standard‑Cfvos att läggas till. |
| [IsCustom](./iscustom/) | Anger om ikonsättet är anpassat. Standardvärdet är falskt. |
| [GetShowValue](./getshowvalue/) | Hämta eller ange flaggan som indikerar om värdena i cellerna som detta ikonsätt tillämpas på ska visas. Standardvärdet är sant. |
| [SetShowValue](./setshowvalue/) | Hämta eller ange flaggan som indikerar om värdena i cellerna som detta ikonsätt tillämpas på ska visas. Standardvärdet är sant. |
| [GetReverse](./getreverse/) | Hämta eller ange flaggan som indikerar om den förvalda ordningen på ikonerna i detta ikonsätt ska vändas. Standardvärdet är falskt. |
| [SetReverse](./setreverse/) | Hämta eller ange flaggan som indikerar om den förvalda ordningen på ikonerna i detta ikonsätt ska vändas. Standardvärdet är falskt. |
