---
title: "PowerQueryFormulaItem.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaItem. Ottiene il valore dell'elemento"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Ottiene il valore dell'elemento.

```csharp
public string Value { get; set; }
```

### Esempi

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

### Vedi anche

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


