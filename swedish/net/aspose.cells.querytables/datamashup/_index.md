---
title: "Klass DataMashup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.DataMashup‑klass. Representerar mashup‑data"
type: docs
url: /sv/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Representerar mashup‑data.

```csharp
public class DataMashup
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Föråldrad.**) Hämtar Power Query‑formelparametrar. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Hämtar alla Power Query‑formler. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till DataMashup-egenskapen i arbetsboken
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Åtkomst till PowerQueryFormulas-egenskapen
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Åtkomst till PowerQueryFormulaParameters-egenskapen
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Exempel på användning: Iterera genom PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Exempel på användning: Iterera genom PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Spara arbetsboken
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


