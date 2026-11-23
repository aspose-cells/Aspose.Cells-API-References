---
title: "PowerQueryFormulaCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaCollection. Obtient PowerQueryFormula par l'index dans la liste"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Obtient [`PowerQueryFormula`](../../powerqueryformula/) par l'index dans la liste.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez les formules Power Query
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Créez et ajoutez une nouvelle formule (si nécessaire)
            // Remarque : L'implémentation réelle peut nécessiter une approche différente pour ajouter des formules
            // À des fins de démonstration, nous travaillerons avec les formules existantes le cas échéant
            if (formulas.Count == 0)
            {
                // Ceci n'est qu'une démonstration - l'API réelle pourrait nécessiter une approche différente
                // pour créer de nouvelles formules
                return;
            }

            // Accédez à la première formule en utilisant la propriété Item
            var formula = formulas[0];
            
            // Obtenez les éléments de formule
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Ceci n'est qu'une démonstration - l'API réelle pourrait nécessiter une approche différente
                // pour créer de nouveaux éléments de formule
                return;
            }

            // Accédez au premier élément en utilisant la propriété Item
            var formulaItem = formulaItems[0];
            
            // Définissez et obtenez la valeur en utilisant la propriété Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Démontrer l'utilisation de la propriété Item
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Enregistrez le classeur
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Obtient [`PowerQueryFormula`](../../powerqueryformula/) par le nom de la formule Power Query.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de l'élément. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créez un classeur en chargeant un fichier existant contenant des formules Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // Obtenez la collection de formules Power Query
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Démontrer l'utilisation de la propriété Item
            try
            {
                // Essayez d'accéder à une formule existante (le cas échéant)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Cela déclenchera une exception pour une formule inexistante
                PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


