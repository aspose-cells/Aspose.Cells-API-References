---
title: "Shape.IsSmartArt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si la forme est un SmartArt"
type: docs
url: /fr/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Indique si la forme est un smart art.

```csharp
public bool IsSmartArt { get; }
```

### Remarques

Uniquement pour le fichier ooxml.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme SmartArt (Remarque : Aspose.Cells n'expose pas directement la création de SmartArt dans les versions actuelles)
            // Pour la démonstration, nous vérifierons les formes existantes
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Vérifier si la forme est SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


