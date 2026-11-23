---
title: "Cells.StandardWidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul en unités de pouces"
type: docs
url: /fr/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces.

```csharp
public double StandardWidthInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la largeur de colonne standard en pouces
            worksheet.Cells.StandardWidthInch = 1.5;

            // Définir la largeur de colonne spécifique en pouces à des fins de démonstration
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Enregistrez le classeur
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


