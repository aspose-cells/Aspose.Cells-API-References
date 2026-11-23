---
title: "CalculationOptions.Recursive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Indique si le calcul des cellules dépendantes doit être effectué de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indique s'il faut calculer les cellules dépendantes de manière récursive lors du calcul d'une cellule qui dépend d'autres cellules. La valeur par défaut est true.

```csharp
public bool Recursive { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyRecursiveDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Créer une référence circulaire
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Premier calcul avec Recursive=true (par défaut)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Deuxième calcul avec Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


