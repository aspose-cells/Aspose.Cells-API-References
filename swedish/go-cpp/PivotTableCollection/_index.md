---
title: "PivotTableCollection-klass"
linktitle: "PivotTableCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotTableCollection-klass. Inkapslar objektet som representerar pivottablecollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Representerar samlingen av alla PivotTable‑objekt på det angivna kalkylbladet.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Utför applikationsdefinierade uppgifter som är kopplade till frigöring, släppande eller återställning av ohanterade resurser. |
| [Add_String_Int_Int](./add_string_int_int/) | Lägger till en ny PivotTable på den angivna rad- och kolumnpositionen i kalkylbladet med standardalternativ. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Lägger till en ny PivotTable med äldre Excel 97-2003-layout och -stil. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Lägger till en ny PivotTable. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Lägger till en ny PivotTable baserad på en annan PivotTable. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Lägger till en ny PivotTable baserad på en annan PivotTable. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Lägger till ett nytt PivotTable-objekt i samlingen med flera konsolideringsområden som datakälla. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Lägger till ett nytt PivotTable-objekt i samlingen med flera konsolideringsområden som datakälla. |
| [Get_Int](./get_int/) | Hämtar PivotTable-rapporten efter index. |
| [Get_String](./get_string/) | Hämtar PivotTable-rapporten efter PivotTables namn. |
| [Get_Int_Int](./get_int_int/) | Hämtar PivotTable-rapporten efter PivotTables position. |
| [Clear](./clear/) | Rensar alla pivottabeller. |
| [Remove_PivotTable](./remove_pivottable/) | Tar bort den angivna PivotTable och raderar PivotTable-data. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Tar bort den angivna PivotTable. |
| [RemoveAt_Int](./removeat_int/) | Tar bort PivotTable på det angivna indexet och raderar PivotTable-data. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Tar bort PivotTable på det angivna indexet. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
