---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataMashup-egenskap. Hämtar power query-formelparametrar"
type: docs
url: /sv/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Hämtar power query-formelparametrar.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället DataMashup.PowerQueryFormulas-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till DataMashup-egenskapen
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Åtkomst till PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Visa antalet parametrar
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Iterera genom parametrarna om några finns
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Spara arbetsboken
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


