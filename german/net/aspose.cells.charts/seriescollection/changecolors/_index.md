---
title: "SeriesCollection.ChangeColors"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection-Methode. Monochromatische Palette für Diagrammreihen festlegen"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Setze eine monochrome Palette für Diagrammserien.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ChartColorPaletteType | Der monochrome Typ. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Daten für das Diagramm befüllen
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Ein Säulendiagramm hinzufügen
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Legen Sie den Datenbereich für die Serie fest
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abrufen der Seriensammlung
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Ändern Sie die Farbpalette aller Serien in der Sammlung.
                // Verwenden Sie einen numerischen Cast zu einem gültigen Enum-Wert (z. B. 0), um abhängige Enum-Mitgliedsnamen zu vermeiden.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Speichern Sie die Arbeitsmappe, um das Ergebnis zu überprüfen
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


