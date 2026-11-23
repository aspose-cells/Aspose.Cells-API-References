---
title: "TextureFill.ImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Obtient et définit les données d'image du remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Obtient et définit les données d'image du remplissage.

```csharp
public byte[] ImageData { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir le type de remplissage de texture
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Charger les données d'image
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Définir les données d'image pour le remplissage de texture
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Enregistrez le classeur
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


