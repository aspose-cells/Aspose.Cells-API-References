---
title: "Klasse ChartPointCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartPointCollection class. Stellt eine Sammlung dar, die alle Punkte einer Serie enthält."
type: docs
url: /de/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Stellt eine Sammlung dar, die alle Punkte in einer Serie enthält.

```csharp
public class ChartPointCollection : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Gibt die Anzahl der Diagrammpunkte zurück. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Gibt das [`ChartPoint`](../chartpoint/)‑Element am angegebenen Index in der Serie zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Alle Einstellungen der Diagrammpunkte entfernen. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Gibt einen Enumerator für die gesamte `ChartPointCollection` zurück. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Entfernt den Punkt am Index der Serie. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ermitteln der Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];

            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von "A1"-Zelle bis "B3"
            chart.NSeries.Add("A1:B3", true);

            // Datenbeschriftungen anzeigen 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Zugriff auf die ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Durchlaufen der Punkte in der Sammlung
            for (int i = 0; i < points.Count; i++)
            {
                // Datenpunkt abrufen
                ChartPoint point = points[i];
                
                // Kuchendiagramm-Explosion festlegen
                point.Explosion = 15;
                
                // Randfarbe festlegen
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Die Excel-Datei speichern
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


