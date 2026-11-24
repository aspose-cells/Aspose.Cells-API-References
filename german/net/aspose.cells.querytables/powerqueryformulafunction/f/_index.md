---
title: "PowerQueryFormulaFunction.F"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaFunction-Eigenschaft. Liest und schreibt die Definition der Funktion"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Liest und setzt die Definition der Funktion.

```csharp
public string F { get; set; }
```

### Beispiele

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
            // Laden Sie eine Arbeitsmappe, die vorhandene Power Query-Formeln enthält
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf die Power Query-Formelsammlung zu
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Rufen Sie eine vorhandene Funktionsformel nach Namen ab
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Wandeln Sie zu PowerQueryFormulaFunction um, um auf die F-Eigenschaft zuzugreifen
            if (formula is PowerQueryFormulaFunction function)
            {
                // Demonstrieren Sie das Abrufen der F-Eigenschaft
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Demonstrieren Sie das Festlegen der F-Eigenschaft
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


