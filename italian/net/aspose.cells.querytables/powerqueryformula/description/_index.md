---
title: "PowerQueryFormula.Description"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene e imposta la descrizione della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Ottiene e imposta la descrizione della formula Power Query.

```csharp
public string Description { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Carica un file esistente con formule Power Query
                workbook = new Workbook("example.xlsx");

                // Accedi alle formule Power Query esistenti
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Visualizza il valore corrente di Description
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Imposta una nuova descrizione
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Salva la cartella di lavoro
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

### Vedi anche

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


