---
title: "Shape.Title"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Spécifie la légende du titre de l'objet forme actuel"
type: docs
url: /fr/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Spécifie le titre (légende) de l'objet forme actuel.

```csharp
public string Title { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Définir le titre de la forme
            shape.Title = "title1";

            // Vérifier que le titre a été défini
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


