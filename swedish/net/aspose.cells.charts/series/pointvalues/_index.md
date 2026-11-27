---
title: "Series.PointValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar de faktiska värdena som används för att plotta varje punkt i denna serie i diagrammet."
type: docs
url: /sv/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

Hämtar de faktiska värdena som används för att plotta varje punkt i denna serie i diagrammet.

```csharp
public ChartDataValue[] PointValues { get; }
```

### Anmärkningar

Denna egenskap ger ett bekvämt sätt att hämta de faktiska värdena som motsvarar data definierade av [`Values`](../values/), särskilt när den angivna datakällan är en extern länk, formel, ...etc.

### Exempel

```csharp
//Demo för att visa ett fall som kräver denna egenskap:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Värden kan vara som "[External.xlsx]Sheet1!$A$1:$A$6" vilket är komplicerat
// för att användaren ska få de faktiska värdena (värdena kan vara länkade till en annan arbetsbok,
// eller cachade i den aktuella arbetsboken). Här kan du använda egenskapen PointValues
// för att hämta de värden som faktiskt visas i Excel-gränssnittet
// i form av en array.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### Se även

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


