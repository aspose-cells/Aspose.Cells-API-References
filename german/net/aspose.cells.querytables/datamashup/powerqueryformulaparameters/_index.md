---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataMashup‑Eigenschaft. Ruft Power‑Query‑Formelparameter ab"
type: docs
url: /de/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Ruft Power‑Query‑Formelparameter ab.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die DataMashup.PowerQueryFormulas‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf die DataMashup‑Eigenschaft zu
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Greifen Sie auf PowerQueryFormulaParameters zu
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Parameteranzahl anzeigen
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Durchlaufen Sie die Parameter, falls welche vorhanden sind
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


