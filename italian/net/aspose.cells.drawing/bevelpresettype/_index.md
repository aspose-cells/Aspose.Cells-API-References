---
title: "Enum BevelPresetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.BevelPresetType. Rappresenta un preset per un tipo di smusso che può essere applicato a una forma in 3D"
type: docs
url: /it/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Rappresenta un preset per un tipo di smussatura che può essere applicato a una forma in 3D.

```csharp
public enum BevelPresetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna smussatura |
| Angle | `1` | Angolo |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Cerchio |
| Convex | `4` | Convesso |
| CoolSlant | `5` | Inclinazione fresca |
| Cross | `6` | Croce |
| Divot | `7` | Incavo |
| HardEdge | `8` | Bordo rigido |
| RelaxedInset | `9` | Inserimento rilassato |
| Riblet | `10` | Ribetto |
| Slope | `11` | Pendenza |
| SoftRound | `12` | Arrotondamento morbido |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Accedi al titolo del grafico e imposta il suo testo
            chart.Title.Text = "Sample Chart with Bevel";

            // Accedi all'area del tracciato del grafico
            PlotArea plotArea = chart.PlotArea;

            // Accedi alle proprietà della forma dell'area del grafico
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Accedi alle proprietà del formato 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accedi alle proprietà dello smusso superiore
            Bevel topBevel = format3D.TopBevel;

            // Imposta il tipo di smusso su "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Imposta la larghezza e l'altezza dello smusso
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Salva la cartella di lavoro
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


