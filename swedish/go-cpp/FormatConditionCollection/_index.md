---
title: "FormatConditionCollection-klass"
linktitle: "FormatConditionCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FormatConditionCollection-klass. Inkapslar objektet som representerar formatconditioncollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Representerar villkorsformatering. FormatConditions kan innehålla upp till tre villkorsformat.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | Lägger till ett formateringsvillkor och påverkad cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorsformat. Referenser till andra blad är inte tillåtna i formlerna för villkorsformatering. |
| [AddArea](./addarea/) | Lägger till ett villkorligt formaterat cellområde. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Lägger till ett formateringsvillkor. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Lägg till ett formatvillkor. |
| [GetCount](./getcount/) | Hämtar antalet villkor. |
| [GetRangeCount](./getrangecount/) | Hämtar antalet villkorligt formaterade områden. |
| [Get](./get/) | Hämtar formateringsvillkoret efter index. |
| [GetCellArea](./getcellarea/) | Hämtar det villkorligt formaterade cellområdet efter index. |
| [RemoveArea_Int](./removearea_int/) | Tar bort det villkorligt formaterade cellområdet efter index. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Ta bort villkorlig formatering i intervallet. |
| [RemoveCondition](./removecondition/) | Tar bort formateringsvillkoret efter index. |
