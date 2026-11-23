---
title: "Shape.Fill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Retourne un objet FillFormat qui contient les propriétés de format de remplissage pour la forme spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Retourne un objet [`FillFormat`](../fillformat/) qui contient les propriétés de format de remplissage pour la forme spécifiée.

```csharp
public FillFormat Fill { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Obtenir le format de remplissage de la forme
            FillFormat fillFmt = shape.Fill;

            // Définissez un remplissage uni avec couleur
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Définir la transparence
            fillFmt.Transparency = 0.5;

            // Enregistrez le classeur
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


