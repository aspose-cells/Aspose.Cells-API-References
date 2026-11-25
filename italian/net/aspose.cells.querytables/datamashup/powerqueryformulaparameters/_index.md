---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataMashup. Restituisce i parametri della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Restituisce i parametri della formula Power Query.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà DataMashup.PowerQueryFormulas. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla proprietà DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Accedi a PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Mostra il conteggio dei parametri
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Itera sui parametri se ne esistono
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


