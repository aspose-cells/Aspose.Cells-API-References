---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Hämtar definitionen av power query-formeln"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Hämtar definitionen av power query-formeln.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Läs in en befintlig arbetsbok med databasanslutningar för att demonstrera PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // Åtkomst till en befintlig anslutning (förutsatt att arbetsboken har minst en anslutning)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Åtkomst till PowerQueryFormula-egenskapen
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // Spara arbetsboken
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


