---
title: "TimelineCollection klass"
linktitle: "TimelineCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "TimelineCollection klass. Inkapslar objektet som representerar timelinecollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/timelinecollection/
---

## TimelineCollection class

Anger samlingen av alla <see cref=\"Timeline\"/>-objekt på kalkylbladet. Det har stödts sedan Excel 2013.

```go

type TimelineCollection struct  {
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
| [Get_Int](./get_int/) | Hämtar Timeline efter index. |
| [Get_String](./get_string/) | Hämtar Timeline efter Timelines namn. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [Add_PivotTable_String_Int](./add_pivottable_string_int/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | Lägg till en ny Timeline med PivotTable som datakälla |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
