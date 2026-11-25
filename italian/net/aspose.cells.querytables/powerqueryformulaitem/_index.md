---
title: "Classe PowerQueryFormulaItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaItem. Rappresenta l'elemento della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Rappresenta l'elemento della formula Power Query.

```csharp
public class PowerQueryFormulaItem
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Ottiene il tipo di questo elemento (Function, Parameter, List, Literal o Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Ottiene il nome dell'elemento. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Ottiene il valore testuale dell'elemento. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Ottiene il valore dell'elemento. |

### Esempi

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
                // Crea un nuovo workbook (può essere un file esistente se disponi di dati Power Query)
                Workbook workbook = new Workbook();

                // Accedi all'oggetto DataMashup che contiene le formule PowerQuery
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Itera attraverso tutte le formule PowerQuery e i loro elementi
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Dimostra la proprietà Name in sola lettura
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Dimostra la proprietà Value in lettura/scrittura
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

### Vedi anche

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


