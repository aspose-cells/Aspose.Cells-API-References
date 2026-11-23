---
title: "Classe PowerQueryFormulaItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaItem. Représente l'élément de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Représente l'élément de la formule Power Query.

```csharp
public class PowerQueryFormulaItem
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Obtient le type de cet élément (Function, Parameter, List, Literal ou Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Obtient le nom de l'élément. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Obtient la valeur texte de l'élément. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Obtient la valeur de l'élément. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur (peut être un fichier existant si vous avez des données Power Query)
                Workbook workbook = new Workbook();

                // Accédez à l'objet DataMashup qui contient les formules PowerQuery
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Itérez à travers toutes les formules PowerQuery et leurs éléments
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Démontrez la propriété Name en lecture seule
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Démontrez la propriété Value en lecture/écriture
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


