---
title: "PowerQueryFormula.Description"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormula-Eigenschaft. Liest und setzt die Beschreibung der Power Query-Formel"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Liest und schreibt die Beschreibung der Power-Query-Formel.

```csharp
public string Description { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Lade eine vorhandene Datei mit Power Query-Formeln
                workbook = new Workbook("example.xlsx");

                // Greife auf vorhandene Power Query-Formeln zu
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Zeige den aktuellen Description-Wert an
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Setze eine neue Beschreibung
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


