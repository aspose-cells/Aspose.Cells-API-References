---
title: "ChartCollection.AddFloatingChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartCollection‑Methode. Fügt ein Diagramm zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Fügt ein Diagramm zur Sammlung hinzu.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ChartType | Diagrammtyp |
| links | Int32 | Der x‑Versatz zur Ecke |
| oben | Int32 | Der y‑Versatz zur Ecke |
| Breite | Int32 | Die Diagrammbreite |
| Höhe | Int32 | Die Diagrammhöhe |

### Rückgabewert

[`Chart`](../../chart/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügt ein schwebendes Diagramm mit angegebenen Abmessungen hinzu
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Beispieldaten zum Diagramm hinzufügen
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


