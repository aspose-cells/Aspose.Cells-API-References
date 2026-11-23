---
title: "Shape.WidthInShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la largeur de la forme en unité de 1/4000 de la forme parente"
type: docs
url: /fr/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

Représente la largeur de la forme, en unité de 1/4000 de la forme parent.

```csharp
public int WidthInShape { get; set; }
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
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer deux formes rectangulaires
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // Regroupez les formes en utilisant des objets forme
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // Démontrez l'utilisation de WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


