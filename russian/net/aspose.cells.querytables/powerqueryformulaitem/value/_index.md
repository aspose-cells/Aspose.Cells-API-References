---
title: "PowerQueryFormulaItem.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaItem. Получает значение элемента"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaitem/value/
---
## PowerQueryFormulaItem.Value property

Получает значение элемента.

```csharp
public string Value { get; set; }
```

### Примеры

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

### См. также

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


