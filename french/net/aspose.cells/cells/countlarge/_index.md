---
title: "Cells.CountLarge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient le nombre total d'objets Cell instanciés"
type: docs
url: /fr/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Obtient le nombre total d'objets Cell instanciés.

```csharp
public long CountLarge { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données aux cellules
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Démontrer la propriété CountLarge
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Afficher la taille du papier pour la démonstration
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


