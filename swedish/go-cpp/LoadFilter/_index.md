---
title: "LoadFilter-klass"
linktitle: "LoadFilter"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LoadFilter-klass. Inkapslar objektet som representerar loadfilter i Go."
type: docs
weight: 200
url: /sv/go-cpp/loadfilter/
---

## LoadFilter class

Representerar filtret som tillhandahåller alternativ för att läsa in data när en arbetsbok laddas från en mall.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Skapar ett LoadFilter med standardfilteralternativen LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Skapar ett LoadFilter med angivna filteralternativ. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Hämtar filteralternativen för att ange vilken data som ska laddas. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Ställer in filteralternativen för att ange vilken data som ska laddas. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Anger bladen (index) och ordning som ska laddas. Standard är null, vilket betyder att alla blad laddas i standardordning i mallfilen. Om inte null och ett bladindex inte finns i den returnerade arrayen, laddas bladet inte. |
| [StartSheet](./startsheet/) | Förbereder filteralternativ innan angivet arbetsblad laddas. Användarens implementation av LoadFilter kan ändra LoadDataFilterOptions här för att ange hur data ska laddas för detta arbetsblad. |
