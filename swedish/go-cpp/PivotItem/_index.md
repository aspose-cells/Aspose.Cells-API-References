---
title: "PivotItem klass"
linktitle: "PivotItem"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotItem klass. Inkapslar objektet som representerar pivotitem i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotitem/
---

## PivotItem class

Representerar ett objekt i en PivotField‑rapport.

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | Hämtar och anger om pivot‑elementet är dolt. |
| [SetIsHidden](./setishidden/) | Hämtar och anger om pivot‑elementet är dolt. |
| [GetPosition](./getposition/) | Anger indexet för detta objekt i alla PivotItems i fältet. |
| [SetPosition](./setposition/) | Anger indexet för detta objekt i alla PivotItems i fältet. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Anger positionsindexet i PivotItems under samma föräldranod. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Anger positionsindexet i PivotItems under samma föräldranod. |
| [Move](./move/) | Flyttar objektet upp eller ner. |
| [IsDetailHidden](./isdetailhidden/) | Hämtar och anger om detaljen för detta pivot‑element är dold. |
| [SetIsDetailHidden](./setisdetailhidden/) | Hämtar och anger om detaljen för detta pivot‑element är dold. |
| [IsCalculatedItem](./iscalculateditem/) | Anger om detta pivot‑element är ett beräknat formel‑element. |
| [GetFormula](./getformula/) | Hämtar formeln för detta beräknade objekt. Fungerar endast när detta objekt är ett beräknat objekt. |
| [IsMissing](./ismissing/) | Anger om objektet togs bort från datakällan. |
| [GetStringValue](./getstringvalue/) | Hämtar strängvärdet för pivot‑elementetIf värdet är null, returneras "" |
| [GetDoubleValue](./getdoublevalue/) | Hämtar dubbelvärdet för pivot‑elementetIf värdet är null eller inte ett tal, returneras 0 |
| [GetDateTimeValue](./getdatetimevalue/) | Hämtar datum‑tidsvärdet för pivot‑elementetIf värdet är null, returneras DateTime.MinValue |
| [GetValue](./getvalue/) | Hämtar värdet för pivot‑elementet |
| [GetName](./getname/) | Hämtar namnet på pivot‑elementet. |
| [SetName](./setname/) | Hämtar namnet på pivot‑elementet. |
