---
title: "FillFormat.GradientColor2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Retourne la couleur de dégradé 2 pour le remplissage spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Renvoie la couleur de dégradé 2 pour le remplissage spécifié.

```csharp
public Color GradientColor2 { get; }
```

### Remarques

Cette propriété n’est pertinente que lorsque le type de couleur de dégradé est GradientColorType.TwoColors.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une forme rectangulaire avec un remplissage en dégradé bicolore
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Vérifier les propriétés de couleur du dégradé
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Voir aussi

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


