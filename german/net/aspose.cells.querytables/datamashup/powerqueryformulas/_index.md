---
title: "DataMashup.PowerQueryFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataMashup‑Eigenschaft. Ruft alle Power‑Query‑Formeln ab"
type: docs
url: /de/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Liest alle Power Query-Formeln.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Beispiele

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
            // Arbeitsmappe mit Power‑Query‑Formeln laden
            Workbook workbook = new Workbook("source.xlsx");
            
            // DataMashup‑Objekt abrufen
            DataMashup mashupData = workbook.DataMashup;
            
            // Prüfen, ob Power‑Query‑Formeln vorhanden sind
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Durchlaufen Sie jede Power‑Query‑Formel
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
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


