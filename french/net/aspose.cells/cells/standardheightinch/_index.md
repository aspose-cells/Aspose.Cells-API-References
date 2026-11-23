---
title: "Cells.StandardHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul en unités de pouces"
type: docs
url: /fr/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pouces.

```csharp
public double StandardHeightInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez la hauteur standard en pouces
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Définissez une nouvelle hauteur standard (1 pouce)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


