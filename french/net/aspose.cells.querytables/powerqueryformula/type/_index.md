---
title: "PowerQueryFormula.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormula. Obtient le type de cette formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Obtient le type de cette formule Power Query.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir les formules existantes (aucune dans le nouveau classeur) pour démontrer la propriété Type
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Dans un scénario réel avec des formules existantes, nous vérifierions leurs types
            Console.WriteLine("Power Query Formula Types:");
            
            // Ceci démontre la vérification de la propriété Type
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // À des fins de démonstration, ajouter une sortie lorsqu'aucune formule n'existe
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Enregistrez le classeur
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


