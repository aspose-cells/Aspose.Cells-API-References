---
title: "PowerQueryFormulaFunction.F"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaFunction. Obtient et définit la définition de la fonction"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Obtient et définit la définition de la fonction.

```csharp
public string F { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Charger un classeur qui contient des formules Power Query existantes
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la collection de formules Power Query
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Récupérer une formule de fonction existante par son nom
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Convertir en PowerQueryFormulaFunction pour accéder à la propriété F
            if (formula is PowerQueryFormulaFunction function)
            {
                // Démontrer la récupération de la propriété F
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Démontrer la définition de la propriété F
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


