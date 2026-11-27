---
title: "Klass PowerQueryFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.PowerQueryFormula class. Representerar definitionen av en Power Query-formel"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Representerar definitionen av en Power Query‑formel.

```csharp
public class PowerQueryFormula
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Hämtar och anger beskrivningen av Power Query-formeln. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Hämtar definitionen av Power Query-formeln. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Hämtar namnet på gruppen som innehåller denna Power Query-formel. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Hämtar och anger namnet på Power Query-formeln. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Hämtar alla objekt i Power Query-formeln. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Hämtar typen av denna Power Query-formel. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Åtkomst till PowerQueryFormulas-samlingen från DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Kontrollera om det finns några befintliga formler
                if (formulas.Count > 0)
                {
                    // Hämta den första PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Visa skrivskyddade egenskaper
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Visa och ändra läs‑skriv‑egenskaper
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Visa antalet formelposter
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


