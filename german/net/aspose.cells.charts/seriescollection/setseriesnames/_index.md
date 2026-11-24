---
title: "SeriesCollection.SetSeriesNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection-Methode. Legt die Namen aller Serien im Diagramm fest"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Setzt die Namen aller Serien im Diagramm.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Index der ersten Serie, deren Namen Sie festlegen möchten. |
| Bereich | String | Gibt den Bereich für den Seriennamen an. |
| isVertical | Boolean | &gt;Gibt an, ob die Serie aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |

### Hinweise

Wenn der Startindex größer ist als die Anzahl der Serien, wird die Methode zurückkehren und nichts tun. Wenn Daten in zusammenhängenden Zellen gesetzt werden, verwenden Sie einen Doppelpunkt zur Trennung, z. B. $C$2:$C$5. Wenn Daten in zusammenhängenden Zellen gesetzt werden, verwenden Sie ein Komma zur Trennung, z. B. ($C$2,$D$5).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Abrufen der Seriensammlung des Diagramms
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Rufen Sie SetSeriesNames mit den Parametern (startIndex: 0, area: "A2:A4", isVertical: true) auf
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Seriendaten hinzufügen
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


