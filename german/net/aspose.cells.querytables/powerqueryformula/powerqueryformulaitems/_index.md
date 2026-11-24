---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormula-Eigenschaft. Gibt alle Elemente der Power Query-Formel zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Liest alle Elemente der Power-Query-Formel.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // Lade die Quellarbeitsmappe
            Workbook workbook = new Workbook("example.xlsx");

            // Greife auf die erste Power Query-Formel und ihr erstes Element zu
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Ändere den Wert des Elements (Laufwerksbuchstaben ersetzen)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Speichere die Arbeitsmappe
            workbook.Save("modified_example.xlsx");

            // Die Änderung überprüfen
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


