---
title: "PowerQueryFormulaItem.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaItem. Obtiene el valor del elemento"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Obtiene el valor del elemento.

```csharp
public string Value { get; set; }
```

### Ejemplos

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

### Ver también

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


