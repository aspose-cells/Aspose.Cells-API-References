---
title: "Classe ShapePropertyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ShapePropertyCollection. Questa classe specifica le proprietà visive della forma per un elemento grafico o una forma"
type: docs
url: /it/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Questa classe specifica le proprietà visive della forma per un elemento o una forma del grafico.

```csharp
public class ShapePropertyCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Rappresenta un oggetto [`Format3D`](./format3d/) che specifica le proprietà 3D della forma per l'elemento grafico o la forma. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Rappresenta un oggetto [`GlowEffect`](./gloweffect/) che specifica l'effetto bagliore per l'elemento grafico o la forma. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Rappresenta un oggetto [`ShadowEffect`](./shadoweffect/) che specifica l'effetto ombra per l'elemento grafico o la forma. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Ottiene e imposta il raggio di sfocatura da applicare ai bordi, in unità di punti. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Cancella le proprietà 3D della forma. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Cancella l'effetto bagliore della forma. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Cancella l'effetto ombra dell'elemento grafico o della forma. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Indica se la forma ha dati di formato 3D. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Indica se la forma ha dati dell'effetto bagliore. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Indica se la forma ha dati dell'effetto ombra. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un grafico di esempio
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Accedi alle proprietà della forma della prima serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configura il formato 3D e lo smusso
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;
            
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Imposta i colori della serie
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


