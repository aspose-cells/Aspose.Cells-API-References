---
title: "RenderingWatermark.IsBackground"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Indique si le filigrane est placé derrière le contenu de la page"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Indique si le filigrane est placé derrière le contenu de la page.

```csharp
public bool IsBackground { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Sample Content");

            // Créer un filigrane avec IsBackground défini sur true
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // Configurer les options d'enregistrement avec filigrane
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Enregistrer avec un filigrane en arrière-plan
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


