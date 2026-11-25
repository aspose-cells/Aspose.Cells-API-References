---
title: "Classe Bevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Bevel. Rappresenta una smussatura di una forma"
type: docs
url: /it/net/aspose.cells.drawing/bevel/
---
## Bevel class

Rappresenta una smussatura di una forma

```csharp
public class Bevel
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Ottiene e imposta l'altezza della smussatura, o quanto sopra la forma viene applicata. In unità di punti. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Ottiene e imposta il tipo di smussatura predefinito. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Ottiene e imposta la larghezza della smussatura, o quanto nella forma viene applicata. In unità di punti. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie di dati al grafico
            chart.NSeries.Add("A1:B4", true);

            // Accedi all'area del tracciato del grafico
            ChartFrame plotArea = chart.PlotArea;

            // Accedi alle proprietà della forma dell'area del grafico
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Accedi alle proprietà del formato 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accedi alle proprietà dello smusso superiore
            Bevel topBevel = format3D.TopBevel;

            // Imposta la larghezza, l'altezza e il tipo della smussatura
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Imposta altre proprietà del formato 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Salva la cartella di lavoro
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


