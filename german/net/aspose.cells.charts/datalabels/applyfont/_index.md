---
title: "DataLabels.ApplyFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Methode. Wendet die Schriftart der Datenbeschriftungen auf alle untergeordneten Knoten an"
type: docs
url: /de/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Wendet die Schriftart der Datenbeschriftungen auf alle untergeordneten Knoten an.

```csharp
public void ApplyFont()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Datenbeschriftungen anzeigen
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Legen Sie eine neue Schriftfarbe für Datenbeschriftungen fest
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Wenden Sie die Schriftarteinstellungen auf alle Datenbeschriftungen an
            series.DataLabels.ApplyFont();
            
            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


