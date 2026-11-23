---
title: "Shape.IsWordArt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si cette forme est un WordArt"
type: docs
url: /fr/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Indique si cette forme est un word art.

```csharp
public bool IsWordArt { get; }
```

### Remarques

Uniquement pour la forme Legacy d'un fichier xls.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme WordArt avec tous les paramètres requis
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Ajouter une forme rectangle régulière avec tous les paramètres requis
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Vérifier si les formes sont des WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // Exemple d'utilisation de la propriété IsWordArt
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


