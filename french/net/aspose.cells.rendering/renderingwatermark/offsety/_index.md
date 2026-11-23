---
title: "RenderingWatermark.OffsetY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient ou définit la valeur de décalage pour VAlignment"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Obtient ou définit la valeur de décalage pour [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Créer la police du filigrane
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Créer un filigrane avec différentes valeurs OffsetY
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // Définir les options d'enregistrement avec filigrane
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Enregistrer avec le décalage du filigrane
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


