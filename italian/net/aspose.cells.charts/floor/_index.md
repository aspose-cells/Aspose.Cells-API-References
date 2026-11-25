---
title: "Classe Floor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.Floor. Incapsula l'oggetto che rappresenta il pavimento di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/floor/
---
## Floor class

Incapsula l'oggetto che rappresenta il pavimento di un grafico 3-D.

```csharp
public class Floor : Area
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo del [`Area`](../../aspose.cells.drawing/area/). (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Ottiene o imposta il bordo del [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Rappresenta un oggetto [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Rappresenta la formattazione dell'area. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 (opaco) a 1.0 (chiaro). (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Istanzia l'oggetto cartella di lavoro
            Workbook workbook = new Workbook();

            // Ottieni la raccolta di celle
            Cells cells = workbook.Worksheets[0].Cells;

            // Inserisci valori nelle celle
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Ottieni la raccolta di grafici
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Aggiungi un nuovo grafico
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Ottieni il grafico appena aggiunto
            Chart chart = charts[index];

            // Imposta nseries del grafico
            chart.NSeries.Add("A1:A3", true);

            // Mostra etichette dati
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Recupera il pavimento del grafico
            Floor floor = chart.Floor;

            // Imposta il bordo del pavimento come rosso
            floor.Border.Color = Color.Red;

            // Imposta formato di riempimento
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Imposta proprietà aggiuntive
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Salva il file
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Vedi anche

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


