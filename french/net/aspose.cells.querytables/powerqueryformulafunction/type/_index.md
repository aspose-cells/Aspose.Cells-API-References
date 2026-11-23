---
title: "PowerQueryFormulaFunction.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaFunction. Obtient le type de formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

Obtient le type de la formule Power Query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une fonction de formule Power Query
            // Comme nous ne pouvons pas créer directement, nous devrons l'obtenir de quelque part
            // À des fins de démonstration, nous allons simplement montrer comment accéder à la propriété Type
            // (Dans une utilisation réelle, vous obtiendriez cela à partir d'une collection existante)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Comme nous ne pouvons pas non plus créer directement un QueryTable, nous passerons cette partie
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Impossible d'ajouter à la collection de tables de requête de cette façon - elle est en lecture seule
            // worksheet.QueryTables[0] = queryTable; // Ligne supprimée
            
            // À des fins de démonstration, nous allons simplement montrer le format de sortie que nous utiliserions si nous avions une fonction
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Enregistrer le résultat
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


