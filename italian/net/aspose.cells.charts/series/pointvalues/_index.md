---
title: "Series.PointValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene i valori effettivi utilizzati per tracciare ogni punto di questa serie nel grafico"
type: docs
url: /it/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Ottiene i valori effettivi utilizzati per tracciare ogni punto di questa serie nel grafico.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Osservazioni

Questa proprietà fornisce un modo comodo per ottenere i valori effettivi corrispondenti ai dati definiti da [`Values`](../values/), soprattutto quando la fonte dati specificata è un collegamento esterno, una formula, ...ecc.

### Esempi

```csharp
//Demo per mostrare un caso che richiede questa proprietà:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// I valori potrebbero essere come "[External.xlsx]Sheet1!$A$1:$A$6" che è complicato
// per l'utente per ottenere i valori effettivi (i valori possono essere collegati a un'altra cartella di lavoro,
// o memorizzati nella cartella di lavoro corrente). Qui è possibile utilizzare la proprietà PointValues
// per ottenere i valori effettivamente visualizzati nell'interfaccia di Excel
// sotto forma di array.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Vedi anche

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


