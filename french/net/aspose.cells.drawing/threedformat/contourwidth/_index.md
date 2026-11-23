---
title: "ThreeDFormat.ContourWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la largeur du contour sur la forme en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Obtient et définit la largeur du contour sur la forme, en unités de points.

```csharp
public double ContourWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Ajoute une forme à la feuille de calcul avec tous les paramètres requis
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // Appliquer le formatage 3D
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Enregistrez le classeur
            wb.Save("output.xlsx");

            // Vérifiez les valeurs enregistrées
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


