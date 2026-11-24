---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaItemCollection‑Eigenschaft. Gibt PowerQueryFormulaItem anhand des Index in der Liste zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Erhält [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) anhand des Index in der Liste.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit einer Vorlage, die Power Query enthält
            Workbook workbook = new Workbook();
            
            // Holen Sie die erste Power Query‑Formel (vorausgesetzt, es existiert eine)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Ändern Sie die Formelelemente mithilfe der Item‑Eigenschaft
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Die Änderung überprüfen
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Erhält [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) anhand des Namens des Elements.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name des Elements. |

### Beispiele

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
                // Laden Sie eine Arbeitsmappe, die Power Query‑Formeln enthält.
                // Ersetzen Sie den Pfad durch eine tatsächliche Datei, die Power Query enthält, falls verfügbar.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Greifen Sie auf die Sammlung von Power Query-Formeln zu.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Holen Sie die erste Power Query-Formel.
                PowerQueryFormula formula = pqFormulas[0];

                // Greifen Sie auf seine Elementsammlung zu.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Rufen Sie das erste Element ab, um einen gültigen Elementnamen zu erhalten.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Verwenden Sie den Item(string)-Indexer (schreibgeschützt), um dasselbe Element nach Namen zu erhalten.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Zeigen Sie die Eigenschaften des abgerufenen Elements an.
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

### Siehe auch

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


