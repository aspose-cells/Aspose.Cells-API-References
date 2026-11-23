---
title: "Shape.AlternativeText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Retourne ou définit la chaîne de texte alternatif descriptif de l'objet Shape"
type: docs
url: /fr/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Retourne ou définit la chaîne de texte descriptif (alternatif) de l'objet [`Shape`](../).

```csharp
public string AlternativeText { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Définir le texte alternatif pour la forme
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Enregistrez le classeur
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


