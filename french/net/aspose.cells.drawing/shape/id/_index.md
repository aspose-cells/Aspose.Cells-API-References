---
title: "Shape.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient l'identifiant de cette forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Obtient l'identifiant de cette forme.

```csharp
public int Id { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Obtenir et afficher l'ID de la forme
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Modifier les propriétés de la forme
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Enregistrez le classeur
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


