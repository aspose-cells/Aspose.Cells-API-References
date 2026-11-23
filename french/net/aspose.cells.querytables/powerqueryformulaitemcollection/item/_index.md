---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaItemCollection. Obtient PowerQueryFormulaItem par l'index dans la liste"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Obtient [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) par l'index dans la liste.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
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
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec un modèle qui contient Power Query
            Workbook workbook = new Workbook();
            
            // Obtenir la première formule Power Query (en supposant qu'elle existe)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Modifier les éléments de formule en utilisant la propriété Item
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Vérifier le changement
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Enregistrez le classeur
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Obtient [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) par le nom de l'élément.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de l'élément. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            try
            {
                // Charger un classeur qui contient des formules Power Query.
                // Remplacer le chemin par un fichier réel contenant Power Query si disponible.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Accéder à la collection de formules Power Query.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Obtenir la première formule Power Query.
                PowerQueryFormula formula = pqFormulas[0];

                // Accéder à sa collection d'éléments.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Récupérer le premier élément pour obtenir un nom d'élément valide.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Utiliser l'indexeur Item(string) (en lecture seule) pour obtenir le même élément par son nom.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Afficher les propriétés de l'élément récupéré.
                Console.WriteLine($"Item Name : {retrievedItem.Name}");
                Console.WriteLine($"Item Value: {retrievedItem.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


