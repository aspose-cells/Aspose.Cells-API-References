---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesLayoutProperties-Eigenschaft. Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwerte verbindet"
type: docs
url: /de/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet.

```csharp
public bool ShowMeanLine { get; set; }
```

### Hinweise

Funktioniert nur für Box‑Whisker-Diagramm.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Box‑Whisker‑Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Ein Box‑Whisker‑Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("A1:A7", true);

            // Erhalte die erste Serie
            Series series = chart.NSeries[0];

            // Auf Layout‑Eigenschaften zugreifen
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Demonstriere die ShowMeanLine‑Eigenschaft
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Setze ShowMeanLine auf true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Speichere die Arbeitsmappe
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


