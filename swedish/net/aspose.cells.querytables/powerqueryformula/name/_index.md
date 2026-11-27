---
title: "PowerQueryFormula.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula property. Hämtar och anger namnet på Power Query-formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Hämtar och anger namnet på Power Query-formeln.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Läs in en befintlig fil med Power Query-formler
            workbook = new Workbook("example.xlsx");
            
            // Åtkomst till befintliga Power Query-formler
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Demonstrera användning av Name‑egenskapen
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Ändra namnet
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Spara arbetsboken
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Se även

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


