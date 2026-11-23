---
title: "RenderingWatermark.Rotation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient ou définit la rotation du filigrane en degrés"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Obtient ou définit la roation du filigrane en degrés.

```csharp
public float Rotation { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Créer une police pour le filigrane
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Créer un filigrane avec rotation
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Définir les options d'enregistrement PDF avec filigrane
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Enregistrer avec filigrane
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


