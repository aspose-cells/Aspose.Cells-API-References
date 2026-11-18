---
title: "NameCollection klass"
linktitle: "NameCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "NameCollection klass. Inkapslar objektet som representerar namecollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/namecollection/
---

## NameCollection class

Representerar en samling av alla <see cref=\"Name\"/>-objekt i kalkylbladet.

```go

type NameCollection struct  {
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
| [Add](./add/) | Definierar ett nytt namn. |
| [Get_Int](./get_int/) | Hämtar Name‑elementet på det angivna indexet. |
| [Filter](./filter/) | Hämtar alla definierade namn efter omfattning. |
| [Get_String](./get_string/) | Hämtar Name‑elementet med det angivna namnet. |
| [Remove_stringArray](./remove_stringarray/) | Ta bort en array av namn |
| [Remove_String](./remove_string/) | Ta bort namnet. |
| [RemoveAt](./removeat/) | Ta bort namnet på det specifika indexet. |
| [Clear](./clear/) | Ta bort alla definierade namn som inte refereras av formlerna och datakällan. Om det definierade namnet refereras, sätter vi bara Name.ReferTo till null och döljer dem. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Ta bort de duplicerade definierade namnen |
| [Sort](./sort/) | Sorterar definierade namn. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
