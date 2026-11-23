---
title: "PowerQueryFormula.Description"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PowerQueryFormula propriété. Obtient et définit la description de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Obtient et définit la description de la formule Power Query.

```csharp
public string Description { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Charger un fichier existant contenant des formules Power Query
                workbook = new Workbook("example.xlsx");

                // Accéder aux formules Power Query existantes
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Afficher la valeur actuelle de Description
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Définir une nouvelle description
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Enregistrez le classeur
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


