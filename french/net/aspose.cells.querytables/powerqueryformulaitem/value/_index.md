---
title: "PowerQueryFormulaItem.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PowerQueryFormulaItem. Obtient la valeur de l'élément"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Obtient la valeur de l'élément.

```csharp
public string Value { get; set; }
```

### Exemples

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

### Voir aussi

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


