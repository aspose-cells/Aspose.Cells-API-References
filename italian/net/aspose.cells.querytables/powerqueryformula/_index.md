---
title: "Classe PowerQueryFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormula. Rappresenta la definizione della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Rappresenta la definizione della formula Power Query.

```csharp
public class PowerQueryFormula
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Ottiene e imposta la descrizione della formula Power Query. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Ottiene la definizione della formula Power Query. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Ottiene il nome del gruppo che contiene questa formula Power Query. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Ottiene e imposta il nome della formula Power Query. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Ottiene tutti gli elementi della formula Power Query. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Ottiene il tipo di questa formula Power Query. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Accedi alla raccolta PowerQueryFormulas da DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Verifica se esistono formule
                if (formulas.Count > 0)
                {
                    // Ottieni la prima PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Visualizza le proprietà in sola lettura
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Visualizza e modifica le proprietà di lettura-scrittura
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Visualizza il conteggio degli elementi della formula
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


