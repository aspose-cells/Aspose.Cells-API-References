---
title: "SeriesCollection-klass"
linktitle: "SeriesCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SeriesCollection-klass. Inkapslar objektet som representerar seriescollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/seriescollection/
---

## SeriesCollection class

Inkapslar en samling av <see cref="Series"/>-objekt.

```go

type SeriesCollection struct  {
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
| [Get](./get/) | Hämtar Series-elementet på det angivna indexet. |
| [GetSeriesByOrder](./getseriesbyorder/) | Hämtar Series-elementet efter ordning. |
| [RemoveAt](./removeat/) | Ta bort en serie på det specifika indexet. |
| [GetCategoryData](./getcategorydata/) | Hämtar eller anger intervallet för kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}"). |
| [SetCategoryData](./setcategorydata/) | Hämtar eller anger intervallet för kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}"). |
| [GetSecondCategoryData](./getsecondcategorydata/) | Hämtar eller anger intervallet för den andra kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10"), eller en sekvens av värden (t.ex. "{2,6,8,10}"). Påverkar endast när vissa serier har plottats på den andra axeln. |
| [SetSecondCategoryData](./setsecondcategorydata/) | Hämtar eller anger intervallet för den andra kategoriaxelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10"), eller en sekvens av värden (t.ex. "{2,6,8,10}"). Påverkar endast när vissa serier har plottats på den andra axeln. |
| [SwapSeries](./swapseries/) | Ändrar direkt ordningen för de två serierna. |
| [SetSeriesNames](./setseriesnames/) | Ställer in namnen på alla serier i diagrammet. |
| [AddR1C1](./addr1c1/) | Lägger till Series-samlingen i ett diagram. |
| [Add_String_Bool](./add_string_bool/) | Lägger till Series-samlingen i ett diagram. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | Lägger till Series-samlingen i ett diagram. |
| [IsColorVaried](./iscolorvaried/) | Anger om färgen på punkterna varierar. |
| [SetIsColorVaried](./setiscolorvaried/) | Anger om färgen på punkterna varierar. |
| [Clear](./clear/) | Rensar samlingen |
| [ChangeColors](./changecolors/) | Ställ in monokromatisk palett för diagramserier. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
