---
title: "ChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartGlobalizationSettings-Methode. Gibt den Namen der Verringerung für die Legende zurück"
type: docs
url: /de/net/aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/
---
## ChartGlobalizationSettings.GetLegendDecreaseName method

Liefert den Namen für 'Abnahme' in der Legende.

```csharp
public virtual string GetLegendDecreaseName()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Globalisierungseinstellungen erstellen und Legendenverringerungsnamen abrufen
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();

            // Gib das Ergebnis aus
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


