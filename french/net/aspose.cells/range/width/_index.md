---
title: "Range.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient la largeur d'une plage en points"
type: docs
url: /fr/net/aspose.cells/range/width/
---
## Range.Width property

Obtient la largeur d'une plage en points.

```csharp
public double Width { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les largeurs de colonne pour démontrer la propriété Width
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Afficher la largeur de la plage (somme des largeurs de colonne dans la plage)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Afficher les propriétés individuelles pour vérification
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


