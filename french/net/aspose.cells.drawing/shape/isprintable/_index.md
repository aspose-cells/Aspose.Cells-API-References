---
title: "Shape.IsPrintable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si l'objet est imprimable. Si False, cette forme ne sera pas imprimée lors de l'impression"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Indique si l'objet est imprimable. Si Faux, cette forme ne sera pas imprimée lors de l'impression.

```csharp
public bool IsPrintable { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Démontrer la propriété IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Basculer la propriété IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Définir IsPrintable à false explicitement
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


