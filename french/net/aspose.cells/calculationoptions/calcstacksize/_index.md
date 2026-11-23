---
title: "CalculationOptions.CalcStackSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200"
type: docs
url: /fr/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

La taille de la pile pour le calcul récursif des cellules. La valeur par défaut est 200.

```csharp
public int CalcStackSize { get; set; }
```

### Remarques

Lorsque un grand nombre de cellules doit être calculé de manière récursive dans l'arbre de dépendances, une StackOverflowException peut survenir pendant le processus de calcul. Dans ce cas, l'utilisateur doit spécifier une valeur plus petite pour cette propriété. Pour une telle situation, l'utilisateur doit déterminer la valeur appropriée pour cette propriété en fonction des formules et des données réelles. Cependant, une valeur trop petite peut entraîner une dégradation des performances du calcul des formules et une valeur inférieure à 2 rendra impossible le calcul d'une formule qui dépend d'une autre. Ainsi, si la valeur spécifiée est inférieure à 2, elle sera réinitialisée à 2.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Mettez en place des formules d'exemple qui nécessitent un calcul de pile
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Calculez avec une taille de pile personnalisée
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


