---
title: "PowerQueryFormulaItem.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaItem-Eigenschaft. Gibt den Wert des Elements zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Ermittelt den Wert des Elements.

```csharp
public string Value { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("source.xlsx");
            
            foreach (PowerQueryFormula formula in workbook.DataMashup.PowerQueryFormulas)
            {
                foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    if (item.Name == "Source")
                    {
                        item.Value = item.Value.Replace("Parameter1", "\"TESTING\"");
                    }
                }
            }
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


