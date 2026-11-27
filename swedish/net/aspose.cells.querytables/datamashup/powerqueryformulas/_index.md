---
title: "DataMashup.PowerQueryFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataMashup-egenskap. Hämtar alla power query-formler"
type: docs
url: /sv/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Hämtar alla Power Query‑formler.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // Läs in arbetsboken med Power Query-formler
            Workbook workbook = new Workbook("source.xlsx");
            
            // Hämta DataMashup-objektet
            DataMashup mashupData = workbook.DataMashup;
            
            // Kontrollera om det finns några Power Query-formler
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Iterera genom varje Power Query-formel
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


