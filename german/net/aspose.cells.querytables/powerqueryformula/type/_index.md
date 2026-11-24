---
title: "PowerQueryFormula.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormula-Eigenschaft. Gibt den Typ dieser Power Query-Formel zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Liest den Typ dieser Power-Query-Formel.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Hole vorhandene Formeln (keine in neuer Arbeitsmappe), um die Type-Eigenschaft zu demonstrieren
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // In einem realen Szenario mit vorhandenen Formeln würden wir ihre Typen prüfen
            Console.WriteLine("Power Query Formula Types:");
            
            // Dies demonstriert das Prüfen der Type-Eigenschaft
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // Zu Demonstrationszwecken füge eine Ausgabe hinzu, wenn keine Formeln existieren
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


