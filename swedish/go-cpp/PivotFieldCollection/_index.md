---
title: "PivotFieldCollection klass"
linktitle: "PivotFieldCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotFieldCollection klass. Inkapslar objektet som representerar pivotfieldcollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Representerar en samling av alla PivotField‑objekt i de olika regionerna i pivottabellen.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | Hämtar PivotFields-typen. |
| [Get_Int](./get_int/) | Hämtar PivotField-objektet vid det specifika indexet. |
| [Get_String](./get_string/) | Hämtar PivotField-objektet med det specifika namnet. |
| [RemoveAt](./removeat/) | Tar bort fält efter index. Endast för filter, rad, kolumn, dataområde. |
| [AddByBaseIndex](./addbybaseindex/) | Lägger till ett PivotField-objekt till den specifika typen PivotFields. |
| [Add](./add/) | Lägger till ett PivotField-objekt till den specifika typen PivotFields. |
| [Insert](./insert/) | Infoga ett pivot-fält vid specifikt index. |
| [Clear](./clear/) | rensa alla fält i PivotFieldCollection |
| [Remove](./remove/) | Tar bort fält från den aktuella regionen. |
| [Move](./move/) | Flyttar PivotField från aktuell position till destinationsposition |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
