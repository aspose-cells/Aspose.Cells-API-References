---
title: "Worksheet.ShowFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique s'il faut afficher les formules ou leurs résultats"
type: docs
url: /fr/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Indique s'il faut afficher les formules ou leurs résultats.

```csharp
public bool ShowFormulas { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la formule dans la cellule A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Afficher initialement la valeur calculée
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Basculer pour afficher le texte de la formule
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


