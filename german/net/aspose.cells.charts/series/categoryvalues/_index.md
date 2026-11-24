---
title: "Series.CategoryValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Liefert die tatsächlichen Kategorienwerte, die zum Plotten jedes Punktes dieser Serie im Diagramm verwendet werden"
type: docs
url: /de/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Liest die tatsächlichen Kategorienwerte, die zum Plotten jedes Punktes dieser Reihe im Diagramm verwendet werden.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Hinweise

Diese Eigenschaft bietet eine bequeme Möglichkeit, die tatsächlichen Werte zu erhalten, die den durch [`XValues`](../xvalues/) definierten Daten entsprechen, insbesondere wenn die angegebene Datenquelle ein externer Link, eine Formel, …etc. ist.

### Beispiele

```csharp
//Demo, um einen Fall zu zeigen, der diese Eigenschaft erfordert:
[C#]

//Eigenständiges Beispiel
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues kann z. B. "[External.xlsx]Sheet1!$B$2:$C$6" sein, was kompliziert ist
// für den Benutzer, um die tatsächlichen Werte zu erhalten (die Werte können mit einer anderen Arbeitsmappe verknüpft sein,
// oder im aktuellen Arbeitsbuch zwischengespeichert). Hier können Sie die CategoryValues‑Eigenschaft verwenden
// um die tatsächlich in der Excel-Oberfläche angezeigten Kategorienwerte zu erhalten
// in Form eines zweidimensionalen Arrays.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Siehe auch

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


