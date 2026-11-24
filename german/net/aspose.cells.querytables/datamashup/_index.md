---
title: "Klasse DataMashup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.DataMashup class. Stellt Mashup-Daten dar"
type: docs
url: /de/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Stellt Mashup-Daten dar.

```csharp
public class DataMashup
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsolete.**) Liest Power Query-Formelparameter. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Liest alle Power Query-Formeln. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die DataMashup‑Eigenschaft der Arbeitsmappe zu
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Greift auf die PowerQueryFormulas‑Eigenschaft zu
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Greift auf die PowerQueryFormulaParameters‑Eigenschaft zu
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Beispielhafte Verwendung: Durchlaufen von PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Beispielhafte Verwendung: Durchlaufen von PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Speichere die Arbeitsmappe
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


