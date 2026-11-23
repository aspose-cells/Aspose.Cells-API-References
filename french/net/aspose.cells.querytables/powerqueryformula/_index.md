---
title: "Classe PowerQueryFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormula. Représente la définition de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Représente la définition de la formule Power Query.

```csharp
public class PowerQueryFormula
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtient et définit la description de la formule Power Query. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Obtient la définition de la formule Power Query. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtient le nom du groupe qui contient cette formule Power Query. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtient et définit le nom de la formule Power Query. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtient tous les éléments de la formule Power Query. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Obtient le type de cette formule Power Query. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Accédez à la collection PowerQueryFormulas depuis DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Vérifiez s'il existe des formules existantes
                if (formulas.Count > 0)
                {
                    // Obtenez la première PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Afficher les propriétés en lecture seule
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Affichez et modifiez les propriétés en lecture‑écriture
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Affichez le nombre d'éléments de formule
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Enregistrez le classeur
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


