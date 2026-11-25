---
title: "Series.CategoryValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene i valori di categoria effettivi utilizzati per tracciare ogni punto di questa serie nel grafico"
type: docs
url: /it/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Ottiene i valori di categoria effettivi utilizzati per tracciare ogni punto di questa serie nel grafico.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Osservazioni

Questa proprietà offre un modo comodo per ottenere i valori effettivi corrispondenti ai dati definiti da [`XValues`](../xvalues/), specialmente quando l'origine dati specificata è un collegamento esterno, una formula, ...etc.

### Esempi

```csharp
//Demo per mostrare un caso che richiede questa proprietà:
[C#]

//Esempio autonomo
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues può essere come "[External.xlsx]Sheet1!$B$2:$C$6" che è complicato
// per l'utente per ottenere i valori effettivi (i valori possono essere collegati a un'altra cartella di lavoro,
// o memorizzato nella cache nella cartella di lavoro corrente). Qui puoi usare la proprietà CategoryValues
// per ottenere i valori di categoria effettivamente visualizzati nell'interfaccia di Excel
// sotto forma di array bidimensionale.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Vedi anche

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


