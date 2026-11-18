---
title: "PivotAreaFilter-klass"
linktitle: "PivotAreaFilter"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotAreaFilter-klass. Inkapslar objektet som representerar pivotareafilter i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

Representerar filtret för <see cref="PivotArea"/> för <see cref="PivotTable"/>.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsSubtotalSet](./issubtotalset/) | Hämtar vilken delsumma som är inställd för detta filter. |
| [SetSubtotals](./setsubtotals/) | Delsumma för filtret. |
| [GetFieldIndex](./getfieldindex/) | Hämtar indexet för fältet i källfälten som detta filter refererar till. Ett värde på -2 indikerar värdefältet. |
| [GetSelected](./getselected/) | Indikerar om detta fält har en markering. Fungerar endast när PivotTable är i översiktsvy. |
| [SetSelected](./setselected/) | Indikerar om detta fält har en markering. Fungerar endast när PivotTable är i översiktsvy. |
