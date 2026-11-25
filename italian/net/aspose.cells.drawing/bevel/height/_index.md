---
title: "Bevel.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Bevel. Ottiene e imposta l'altezza del bevel o quanto sopra la forma viene applicato. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Ottiene e imposta l'altezza della smussatura, o quanto sopra la forma viene applicata. In unità di punti.

```csharp
public double Height { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Accedi al formato 3D dell'area del grafico
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Configura il bevel superiore con la proprietà Height
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Salva la cartella di lavoro
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


