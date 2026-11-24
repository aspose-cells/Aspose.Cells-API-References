---
title: "Series.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt den Namen der Datenserie zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/series/name/
---
## Series.Name property

Liest oder setzt den Namen der Datenserie.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("A2:C2", true);
            
            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            // 1. Referenzname zu einer Zelle
            chart.NSeries[0].Name = "=A1";
            
            // 2. Setze einen String als Namen
            chart.NSeries[0].Name = "First Series";
            
            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


