---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaItemCollection. Ottiene PowerQueryFormulaItem per indice nell'elenco"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Ottiene [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) per indice nell'elenco.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con un modello che contiene Power Query
            Workbook workbook = new Workbook();
            
            // Ottieni la prima formula Power Query (presumendo che ne esista una)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Modifica gli elementi della formula usando la proprietà Item
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Verifica la modifica
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Ottiene [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) per nome dell'elemento.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome dell'elemento. |

### Esempi

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
                // Carica un workbook che contiene formule Power Query.
                // Sostituisci il percorso con un file reale contenente Power Query, se disponibile.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Accedi alla raccolta di formule Power Query.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Ottieni la prima formula Power Query.
                PowerQueryFormula formula = pqFormulas[0];

                // Accedi alla sua raccolta di elementi.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Recupera il primo elemento per ottenere un nome di elemento valido.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Usa l'indicizzatore Item(string) (di sola lettura) per ottenere lo stesso elemento per nome.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Visualizza le proprietà dell'elemento recuperato.
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

### Vedi anche

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


