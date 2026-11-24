---
title: "DisplayUnitLabel.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DisplayUnitLabel‑Eigenschaft. Gibt den Text der Anzeigeeinheitsbeschriftung zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Liest oder legt fest den Text des Anzeigeeinheiten‑Labels.

```csharp
public override string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A1:A4", true);
            
            // Konfiguriere die Anzeigeeinheitsbeschriftung
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Greife zu und ändere den Text der Anzeigeeinheitsbeschriftung
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Ändere den Text
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Speichere die Arbeitsmappe
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


