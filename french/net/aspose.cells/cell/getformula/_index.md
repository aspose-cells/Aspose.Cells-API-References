---
title: "Cell.GetFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtenir la formule de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Obtenir la formule de cette cellule.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Valeur de retour

la formule de cette cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et des formules
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.PutValue(10);
            
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.PutValue(20);
            
            Cell cellC1 = worksheet.Cells["C1"];
            cellC1.Formula = "=A1+B1";
            
            // Démontrer GetFormula avec différents paramètres
            Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
            Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
            
            // Modifier le style de formule en local et montrer la différence
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
            Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


