---
title: "Classe Format3D"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Format3D. Questa classe specifica le proprietà della forma 3D per un elemento o una forma del grafico"
type: docs
url: /it/net/aspose.cells.drawing/format3d/
---
## Format3D class

Questa classe specifica le proprietà della forma 3D per un elemento o una forma del grafico.

```csharp
public class Format3D
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Ottiene e imposta l'angolo di illuminazione. Intervallo da 0 a 359,9 gradi. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Ottiene e imposta il tipo di illuminazione da applicare alla scena della forma. Il valore predefinito è LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Ottiene e imposta il tipo di materiale che, combinato con le proprietà di illuminazione, conferisce l'aspetto finale a una forma. Il valore predefinito è PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Ottiene l'oggetto [`Bevel`](../bevel/) che contiene le proprietà associate alla definizione di una smussatura sulla parte superiore o frontale di una forma. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Indica se la forma ha dati di smussatura superiore. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            chart.NSeries.Add("A1:A4", true);

            // Accedi alla prima serie
            Series series = chart.NSeries[0];

            // Accedi al formato 3D della serie
            Format3D format3D = series.ShapeProperties.Format3D;

            // Imposta le proprietà del formato 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Verifica se la forma ha dati di smussatura superiore
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Salva la cartella di lavoro
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


