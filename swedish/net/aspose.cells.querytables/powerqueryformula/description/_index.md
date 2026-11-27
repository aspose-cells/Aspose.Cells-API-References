---
title: "PowerQueryFormula.Description"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula property. Hämtar och anger beskrivningen av Power Query-formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Hämtar och anger beskrivningen av Power Query-formeln.

```csharp
public string Description { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Läs in en befintlig fil med Power Query-formler
                workbook = new Workbook("example.xlsx");

                // Åtkomst till befintliga Power Query-formler
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Visa det aktuella Description‑värdet
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Ange en ny beskrivning
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Spara arbetsboken
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

### Se även

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


