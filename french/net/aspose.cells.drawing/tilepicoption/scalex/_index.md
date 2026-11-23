---
title: "TilePicOption.ScaleX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TilePicOption. Obtient ou définit l'échelle X pour le carrelage de l'image"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

Obtient ou définit l'échelle X de l'image en mosaïque.

```csharp
public double ScaleX { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et créer un graphique
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Définissez le remplissage de texture avec l'image
            string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            
            // Démontrer la propriété ScaleX
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling

            // Enregistrez le classeur
            workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
        }
    }
}
```

### Voir aussi

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


