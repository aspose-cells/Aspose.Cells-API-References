---
title: "Range.Left"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient la distance en points du bord gauche de la colonne A au bord gauche de la plage"
type: docs
url: /fr/net/aspose.cells/range/left/
---
## Range.Left property

Obtient la distance, en points, du bord gauche de la colonne A au bord gauche de la plage.

```csharp
public double Left { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage de B2 à C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Démontrer l'utilisation de la propriété Left
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Calculer les valeurs attendues en fonction du cas de test
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


