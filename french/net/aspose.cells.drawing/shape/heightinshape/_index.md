---
title: "Shape.HeightInShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente"
type: docs
url: /fr/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent.

```csharp
public int HeightInShape { get; set; }
```

### Remarques

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter d'abord les formes avec tous les paramètres requis
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // Grouper les formes
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // Définir la hauteur du rectangle relative à la forme groupe parente (1/4000 de la hauteur du parent)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // Enregistrez le classeur
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


