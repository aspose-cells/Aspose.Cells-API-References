---
title: "ChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartGlobalizationSettings‑Methode. Gibt den Namen der „Other“-Beschriftungen für das Diagramm zurück"
type: docs
url: /de/net/aspose.cells.charts/chartglobalizationsettings/getothername/
---
## ChartGlobalizationSettings.GetOtherName method

Ermittelt den Namen der "Other"-Beschriftungen für das Diagramm.

```csharp
public virtual string GetOtherName()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetOtherNameDemo
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

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Globalisierungs­einstellungen erstellen und anderen Namen abrufen
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string otherName = globalizationSettings.GetOtherName();

            // Gib das Ergebnis aus
            Console.WriteLine("Other Name: " + otherName);

            // Arbeitsmappe speichern.
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


