---
title: "Series.PointValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt die tatsächlichen Werte zurück, die verwendet werden, um jeden Punkt dieser Serie im Diagramm zu plotten."
type: docs
url: /de/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Liefert die tatsächlichen Werte, die zum Plotten jedes Punktes dieser Serie im Diagramm verwendet werden.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Hinweise

Diese Eigenschaft bietet eine bequeme Möglichkeit, die tatsächlichen Werte zu erhalten, die den durch [`Values`](../values/) definierten Daten entsprechen, insbesondere wenn die angegebene Datenquelle ein externer Link, eine Formel usw. ist.

### Beispiele

```csharp
//Demo, um einen Fall zu zeigen, der diese Eigenschaft erfordert:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Values könnte z. B. "[External.xlsx]Sheet1!$A$1:$A$6" sein, was kompliziert ist.
// für den Benutzer, um die tatsächlichen Werte zu erhalten (die Werte können mit einer anderen Arbeitsmappe verknüpft sein,
// oder im aktuellen Arbeitsbuch zwischengespeichert sein). Hier können Sie die PointValues‑Eigenschaft verwenden.
// um die tatsächlich in der Excel-Oberfläche angezeigten Werte zu erhalten
// in Form eines Arrays.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Siehe auch

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


