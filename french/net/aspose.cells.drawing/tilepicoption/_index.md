---
title: "Classe TilePicOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.TilePicOption. Représente l'image en mosaïque comme texture"
type: docs
url: /fr/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Représente l'image en mosaïque comme texture.

```csharp
public class TilePicOption
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Obtient ou définit l'alignement du carrelage. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Obtient ou définit le type de miroir pour le carrelage. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Obtient ou définit le décalage X de l'image en mosaïque. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Obtient ou définit le décalage Y de l'image en mosaïque. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Obtient ou définit l'échelle X de l'image en mosaïque. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Obtient ou définit l'échelle Y de l'image en mosaïque. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un graphique pour la démonstration
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir le type de remplissage sur texture
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Charger l'image d'exemple (remplacer par le chemin réel)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Créer et configurer TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Enregistrez le classeur
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


