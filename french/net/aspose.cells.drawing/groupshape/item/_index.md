---
title: "GroupShape.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GroupShape. Obtient la forme enfant par indice"
type: docs
url: /fr/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Obtient la forme enfant par indice.

```csharp
public Shape this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | l'indice de la forme enfant. |

### Valeur de retour

renvoie la forme enfant.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux formes rectangulaires
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Grouper les formes
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Accéder et afficher les propriétés de la première forme
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Modifier les propriétés de la première forme via l'accès Item
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Accéder et modifier la deuxième forme directement via l'indexeur
            groupShape[1].Text = "Second Grouped Shape";

            // Vérifier les modifications
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Enregistrer le classeur modifié
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


