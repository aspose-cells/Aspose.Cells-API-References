---
title: "Cell.Calculate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Calcule la formule de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calcule la formule de la cellule.

```csharp
public void Calculate(CalculationOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options de calcul |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir une formule simple dans la cellule A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Calculer avec les options par défaut
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Définir une formule matricielle dans la plage B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Calculer la formule matricielle avec des options
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Définir une formule plus complexe dans la cellule A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Calculer avec des options
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


