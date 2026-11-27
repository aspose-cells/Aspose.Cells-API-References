---
title: "PowerQueryFormulaFunction.F"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaFunction-egenskap. Hämtar och anger definitionen av funktionen."
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Hämtar och anger definitionen av funktionen.

```csharp
public string F { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Läs in en arbetsbok som innehåller befintliga Power Query-formler.
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till samlingen av Power Query-formler.
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Hämta en befintlig funktionsformel efter namn.
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Kasta till PowerQueryFormulaFunction för att komma åt F-egenskapen.
            if (formula is PowerQueryFormulaFunction function)
            {
                // Visa hur man hämtar F-egenskapen.
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Visa hur man anger F-egenskapen.
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


