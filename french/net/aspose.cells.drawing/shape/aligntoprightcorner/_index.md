---
title: "Shape.AlignTopRightCorner"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape method. Déplace l'image vers le coin supérieur droit"
type: docs
url: /fr/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Déplace l'image vers le coin supérieur droit.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | l'index de la ligne. |
| rightColumn | Int32 | l'index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape d'exemple à aligner
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Alignez le coin supérieur droit du shape à la ligne 2, colonne 5
            shape.AlignTopRightCorner(2, 5);

            // Enregistrez le classeur
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


