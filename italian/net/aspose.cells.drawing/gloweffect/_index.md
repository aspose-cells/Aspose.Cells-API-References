---
title: "Classe GlowEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.GlowEffect. Questa classe specifica un effetto bagliore in cui un contorno sfocato di colore è aggiunto al di fuori dei bordi dell'oggetto"
type: docs
url: /it/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Questa classe specifica un effetto bagliore, in cui un contorno sfocato di colore viene aggiunto al di fuori dei bordi dell'oggetto.

```csharp
public class GlowEffect
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Ottiene il colore dell'effetto bagliore. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Ottiene e imposta il raggio del bagliore, in unità di punti. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Ottiene e imposta il raggio del bagliore, in unità di punti. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Ottiene e imposta il grado di trasparenza dell'effetto bagliore. Intervallo da 0,0 (opaco) a 1,0 (trasparente). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ad arco al foglio di lavoro
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Imposta la posizione dell'arco
            arcShape.Placement = PlacementType.FreeFloating;

            // Imposta il formato di riempimento
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Imposta lo stile della linea
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Crea un'istanza di GlowEffect e imposta le sue proprietà
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Salva la cartella di lavoro
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


