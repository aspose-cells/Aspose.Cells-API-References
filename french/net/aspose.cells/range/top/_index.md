---
title: "Range.Top"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient la distance en points entre le bord supérieur de la ligne 1 et le bord supérieur de la plage"
type: docs
url: /fr/net/aspose.cells/range/top/
---
## Range.Top property

Obtient la distance, en points, du bord supérieur de la ligne 1 au bord supérieur de la plage.

```csharp
public double Top { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage et définir quelques valeurs
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Démontrer l'utilisation de la propriété Top
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


