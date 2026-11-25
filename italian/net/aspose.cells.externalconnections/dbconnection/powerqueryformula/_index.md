---
title: "DBConnection.PowerQueryFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. Ottiene la definizione della formula di Power Query"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Ottiene la definizione della formula Power Query.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;

    public class DBConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla raccolta di connessioni esterne
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Trova il primo DBConnection nella raccolta (se presente)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Accedi alla proprietà PowerQueryFormula (sola lettura)
                    PowerQueryFormula powerQueryFormula = dbConn.PowerQueryFormula;

                    if (powerQueryFormula != null)
                    {
                        // Visualizza le proprietà di PowerQueryFormula
                        Console.WriteLine("PowerQueryFormula Type: " + powerQueryFormula.Type);
                        Console.WriteLine("PowerQueryFormula GroupName: " + powerQueryFormula.GroupName);
                        Console.WriteLine("PowerQueryFormula FormulaDefinition: " + powerQueryFormula.FormulaDefinition);
                        Console.WriteLine("PowerQueryFormula Name: " + powerQueryFormula.Name);
                        Console.WriteLine("PowerQueryFormula Description: " + powerQueryFormula.Description);

                        // Dimostra l'accesso alla raccolta PowerQueryFormulaItems
                        Console.WriteLine("Number of PowerQueryFormulaItems: " + powerQueryFormula.PowerQueryFormulaItems.Count);
                    }
                    else
                    {
                        Console.WriteLine("PowerQueryFormula is null for this connection.");
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved as PowerQueryFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


