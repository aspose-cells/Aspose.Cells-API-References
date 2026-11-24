---
title: "Klasse PowerQueryFormulaItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaItem Klasse. Stellt das Element der Power‑Query‑Formel dar"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Stellt das Element der Power‑Query‑Formel dar.

```csharp
public class PowerQueryFormulaItem
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Ermittelt den Typ dieses Elements (Function, Parameter, List, Literal oder Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Ermittelt den Namen des Elements. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Ermittelt den Textwert des Elements. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Ermittelt den Wert des Elements. |

### Beispiele

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
                // Erstellen Sie eine neue Arbeitsmappe (kann eine vorhandene Datei sein, wenn Sie Power‑Query‑Daten haben)
                Workbook workbook = new Workbook();

                // Greifen Sie auf das DataMashup‑Objekt zu, das PowerQuery‑Formeln enthält
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Durchlaufen Sie alle PowerQuery‑Formeln und deren Elemente
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Demonstration der schreibgeschützten Name‑Eigenschaft
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Demonstration der Lese/Schreib‑Value‑Eigenschaft
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

### Siehe auch

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


