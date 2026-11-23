---
title: "Cell.FormulaLocal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la formule formatée selon la locale de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Obtenez la formule formatée selon la locale de la cellule.

```csharp
public string FormulaLocal { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la locale par défaut sur l'allemand pour la démonstration
            workbook.Settings.Region = CountryCode.Germany;
            
            // Accéder à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            
            // Définir la formule au format standard (anglais)
            cell.Formula = "=SUM(B1:C1)";
            
            // Afficher les formules aux formats standard et local
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Définir la formule au format local (allemand)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Afficher à nouveau les formules pour montrer la différence
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Démontrer GetFormula avec la localisation
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


