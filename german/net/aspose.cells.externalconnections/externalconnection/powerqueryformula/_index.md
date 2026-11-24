---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection‑Eigenschaft. Gibt die Definition der Power‑Query‑Formel zurück."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Ruft die Definition der Power‑Query‑Formel ab.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Laden Sie eine vorhandene Arbeitsmappe mit Datenverbindungen, um PowerQueryFormula zu demonstrieren.
            workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf eine vorhandene Verbindung zu (unter der Annahme, dass die Arbeitsmappe mindestens eine Verbindung hat)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Greifen Sie auf die PowerQueryFormula‑Eigenschaft zu
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
            
            // Speichere die Arbeitsmappe
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


