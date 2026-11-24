---
title: "Chart.ChangeTemplate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Ändert den Diagrammtyp mit einer vordefinierten Vorlage"
type: docs
url: /de/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Diagrammtyp mit einer vordefinierten Vorlage ändern.

```csharp
public void ChangeTemplate(byte[] data)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Daten | Byte[] | Die Daten der Diagrammvorlagendatei (.crtx). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:B4", false);

            // Vorlagendaten aus einer anderen Diagrammdatei abrufen
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Rufen Sie die ChangeTemplate‑Methode mit einem Byte‑Array-Parameter auf
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Effekt durch Speichern der Arbeitsmappe zeigen
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


