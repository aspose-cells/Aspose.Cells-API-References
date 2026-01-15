---
title: PowerQueryFormulaItemCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormulaItemCollection property. Gets PowerQueryFormulaItem by the index in the list
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the index in the list.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook with a template that contains Power Query
            Workbook workbook = new Workbook();
            
            // Get the first Power Query formula (assuming one exists)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Modify the formula items using Item property
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Verify the change
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Save the workbook
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### See Also

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Gets [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) by the name of the item.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the item. |

### Examples

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
                // Load a workbook that contains Power Query formulas.
                // Replace the path with an actual file containing Power Query if available.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Access the collection of Power Query formulas.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Get the first Power Query formula.
                PowerQueryFormula formula = pqFormulas[0];

                // Access its items collection.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Retrieve the first item to obtain a valid item name.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Use the Item(string) indexer (read‑only) to get the same item by name.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Display the retrieved item's properties.
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

### See Also

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


