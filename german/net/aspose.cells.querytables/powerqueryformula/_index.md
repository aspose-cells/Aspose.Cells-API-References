---
title: "Klasse PowerQueryFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormula-Klasse. Stellt die Definition einer Power-Query-Formel dar."
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Stellt die Definition einer Power‑Query‑Formel dar.

```csharp
public class PowerQueryFormula
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Liest und schreibt die Beschreibung der Power-Query-Formel. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Liest die Definition der Power-Query-Formel. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Liest den Namen der Gruppe, die diese Power-Query-Formel enthält. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Liest und schreibt den Namen der Power-Query-Formel. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Liest alle Elemente der Power-Query-Formel. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Liest den Typ dieser Power-Query-Formel. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Zugriff auf die PowerQueryFormulas-Sammlung von DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Prüfen, ob bereits Formeln vorhanden sind
                if (formulas.Count > 0)
                {
                    // Holen Sie die erste PowerQueryFormula ab
                    PowerQueryFormula formula = formulas[0];

                    // Zeige schreibgeschützte Eigenschaften an
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Anzeigen und Ändern von Lese‑Schreib‑Eigenschaften
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Anzahl der Formelelemente anzeigen
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


