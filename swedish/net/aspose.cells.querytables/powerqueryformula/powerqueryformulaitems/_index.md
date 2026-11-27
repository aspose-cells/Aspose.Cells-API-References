---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula property. Hämtar alla objekt i Power Query-formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Hämtar alla objekt i Power Query-formeln.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Exempel

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
            // Läs in källarbetsboken
            Workbook workbook = new Workbook("example.xlsx");

            // Åtkomst till den första Power Query-formeln och dess första objekt
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Ändra objektvärdet (byt ut enhetsbokstaven)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Spara arbetsboken
            workbook.Save("modified_example.xlsx");

            // Verifiera ändringen
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Se även

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


