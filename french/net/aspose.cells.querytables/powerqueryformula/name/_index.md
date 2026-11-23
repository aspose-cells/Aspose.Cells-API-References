---
title: "PowerQueryFormula.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormula. Obtient et définit le nom de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Obtient et définit le nom de la formule Power Query.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Charger un fichier existant contenant des formules Power Query
            workbook = new Workbook("example.xlsx");
            
            // Accéder aux formules Power Query existantes
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Démontrer l'utilisation de la propriété Name
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Modifier le nom
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Enregistrez le classeur
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


