---
title: "Series.CategoryValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar de faktiska kategorivärdena som används för att plotta varje punkt i denna serie i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

Hämtar de faktiska kategorivärdena som används för att plotta varje punkt i denna serie i diagrammet.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### Anmärkningar

Denna egenskap ger ett bekvämt sätt att hämta de faktiska värdena som motsvarar data definierade av [`XValues`](../xvalues/), särskilt när den angivna datakällan är en extern länk, formel, ...etc.

### Exempel

```csharp
//Demo för att visa ett fall som kräver denna egenskap:
[C#]

//Fristående exempel
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues kan vara som "[External.xlsx]Sheet1!$B$2:$C$6" vilket är komplicerat
// för att användaren ska få de faktiska värdena (värdena kan vara länkade till en annan arbetsbok,
// eller cachade i den aktuella arbetsboken). Här kan du använda egenskapen CategoryValues
// för att hämta de kategorivärden som faktiskt visas i Excel-gränssnittet
// i form av en tvådimensionell matris.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### Se även

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


