---
title: "TilePicOption.ScaleY"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TilePicOption. Obtient ou définit l'échelle Y pour l'image en mosaïque"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Obtient ou définit l'échelle Y de l'image en mosaïque.

```csharp
public double ScaleY { get; set; }
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
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définissez le remplissage de texture avec l'image
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // Configurez les options de mosaïque avec ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Enregistrez le classeur
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


