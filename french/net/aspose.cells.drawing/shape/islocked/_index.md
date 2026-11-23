---
title: "Shape.IsLocked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est pertinente que si la feuille de calcul ou les objets dans la feuille de calcul sont protégés"
type: docs
url: /fr/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

Vrai signifie que l'objet ne peut pas être modifié lorsque la feuille est protégée. Notez que cette valeur n'est significative que si la feuille de calcul ou les objets de la feuille de calcul sont protégés.

```csharp
public bool IsLocked { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Protéger la feuille de calcul
            worksheet.Protect(ProtectionType.All);

            // Démontrer le verrouillage/déverrouillage de la forme
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Déverrouiller la forme
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Verrouiller la forme
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


