---
title: "DataMashup.PowerQueryFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataMashup. Возвращает все формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Получает все формулы Power Query.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Примеры

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
            // Загрузить книгу с формулами Power Query
            Workbook workbook = new Workbook("source.xlsx");
            
            // Получить объект DataMashup
            DataMashup mashupData = workbook.DataMashup;
            
            // Проверьте, есть ли какие‑либо формулы Power Query
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Переберите каждую формулу Power Query
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
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


