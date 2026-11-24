---
title: "ChartGlobalizationSettings.GetAxisTitleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartGlobalizationSettings-Methode. Gibt den Namen des Titels für die Achse zurück"
type: docs
url: /de/net/aspose.cells.charts/chartglobalizationsettings/getaxistitlename/
---
## ChartGlobalizationSettings.GetAxisTitleName method

Liefert den Namen des Titels für die Achse.

```csharp
public virtual string GetAxisTitleName()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Globalisierungseinstellungen erstellen und Achsentitelnamen abrufen
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string axisTitleName = globalizationSettings.GetAxisTitleName();

            // Achsentitel festlegen
            chart.ValueAxis.Title.Text = axisTitleName;
            chart.CategoryAxis.Title.Text = axisTitleName;

            // Ausgabe des Achsentitelnamens
            Console.WriteLine("Axis Title Name: " + axisTitleName);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


