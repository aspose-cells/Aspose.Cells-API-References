---
title: "Cell.IsErrorValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Vérifie si la valeur de cette cellule est une erreur"
type: docs
url: /fr/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Vérifie si la valeur de cette cellule est une erreur.

```csharp
public bool IsErrorValue { get; }
```

### Remarques

S’applique également aux cellules de formule pour vérifier si le résultat calculé est une erreur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir une formule qui entraînera une erreur
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // Calculer les formules
            workbook.CalculateFormula();

            // Démontrer la propriété IsErrorValue
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // Définir une valeur valide
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // Définir une erreur SPILL (erreur de formule de tableau dynamique Excel 365+)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


