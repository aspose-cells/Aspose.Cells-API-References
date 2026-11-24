---
title: "PowerQueryFormula.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormula-Eigenschaft. Liest und setzt den Namen der Power Query-Formel"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Liest und schreibt den Namen der Power-Query-Formel.

```csharp
public string Name { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Lade eine vorhandene Datei mit Power Query-Formeln
            workbook = new Workbook("example.xlsx");
            
            // Greife auf vorhandene Power Query-Formeln zu
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Demonstrieren Sie die Verwendung der Name-Eigenschaft
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Ändere den Namen
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


