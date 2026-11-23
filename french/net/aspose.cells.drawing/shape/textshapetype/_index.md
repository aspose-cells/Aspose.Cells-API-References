---
title: "Shape.TextShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape property. Obtient et définit le type de forme texte prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Obtient et définit le type de forme texte prédéfini.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Vérifier et définir TextShapeType si inconnu
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Afficher le TextShapeType de la forme
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### Voir aussi

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


