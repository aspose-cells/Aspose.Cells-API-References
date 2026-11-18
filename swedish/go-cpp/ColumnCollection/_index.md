---
title: "ColumnCollection klass"
linktitle: "ColumnCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ColumnCollection klass. Inkapslar objektet som representerar columncollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/columncollection/
---

## ColumnCollection class

Samlingsobjektet av <see cref="Column"/>‑objekt som representerar de individuella kolumninställningarna i ett kalkylblad. Column‑objektet representerar endast inställningar såsom kolumnbredd, stilar, osv. för hela kolumnen och har inget att göra med om det finns icke‑tomma celler (data) i motsvarande kolumn. Och "Count" för denna samling representerar endast antalet Column‑objekt som har instansierats i samlingen, och har inget att göra med om det finns icke‑tomma celler (data) i kalkylbladet.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | Hämtar Column-objektet efter positionen i listan. |
| [Get](./get/) | Hämtar ett Column-objekt efter kolumnindex. Column-objektet för angivet kolumnindex kommer att instansieras om det inte redan finns. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
