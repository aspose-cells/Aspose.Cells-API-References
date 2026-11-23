---
title: "Shape.GetResultOfSmartArt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Conversion du smart art en formes groupées"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Conversion du smart art en formes groupées.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle (puisque nous ne pouvons pas créer de SmartArt directement)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // Dans un scénario réel, nous chargerions une forme SmartArt existante
            // À des fins de démonstration, nous passerons le contrôle IsSmartArt car nous ne pouvons pas le définir

            // Obtenir le résultat du SmartArt (ne fonctionnerait que si la forme était réellement un SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Voir aussi

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


