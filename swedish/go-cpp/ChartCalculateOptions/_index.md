---
title: "ChartCalculateOptions klass"
linktitle: "ChartCalculateOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ChartCalculateOptions klass. Inkapslar objektet som representerar chartcalculateoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/chartcalculateoptions/
---

## ChartCalculateOptions class

Representerar alternativen för att beräkna ett diagram.

```go

type ChartCalculateOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewChartCalculateOptions](./newchartcalculateoptions/) | Skapar alternativen för att beräkna diagram. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetUpdateAllPoints](./getupdateallpoints/) | Om alla datapunkter ska uppdateras vid diagramberäkning. Standard: False. När du vill få värdet för varje datapunkt i diagrammet specifikt, sätt den till true. Om denna parameter är satt till True kan nya datapunkter genereras när diagrammet beräknas. Detta kan göra Excel-filen större. |
| [SetUpdateAllPoints](./setupdateallpoints/) | Om alla datapunkter ska uppdateras vid diagramberäkning. Standard: False. När du vill få värdet för varje datapunkt i diagrammet specifikt, sätt den till true. Om denna parameter är satt till True kan nya datapunkter genereras när diagrammet beräknas. Detta kan göra Excel-filen större. |
