---
title: "DataMashup.PowerQueryFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataMashup. Obtient toutes les formules Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Récupère toutes les formules Power Query.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // Charger le classeur avec des formules Power Query
            Workbook workbook = new Workbook("source.xlsx");
            
            // Obtenir l'objet DataMashup
            DataMashup mashupData = workbook.DataMashup;
            
            // Vérifiez s'il existe des formules Power Query
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Itérez à travers chaque formule Power Query
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


