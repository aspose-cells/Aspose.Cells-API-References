---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene la definizione della formula Power Query"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Ottiene la definizione della formula Power Query.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Carica una cartella di lavoro esistente con connessioni dati per dimostrare PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // Accedi a una connessione esistente (supponendo che la cartella di lavoro abbia almeno una connessione)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Accedi alla proprietà PowerQueryFormula
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
            
            // Salva la cartella di lavoro
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


