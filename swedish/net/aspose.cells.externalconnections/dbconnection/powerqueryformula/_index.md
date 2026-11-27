---
title: "DBConnection.PowerQueryFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection egenskap. Hämtar definitionen av power query‑formeln."
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Hämtar definitionen av power query-formeln.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till samlingen av externa anslutningar.
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Hitta den första DBConnection i samlingen (om någon).
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
                    // Åtkomst till PowerQueryFormula‑egenskapen (skrivskyddad).
                    PowerQueryFormula powerQueryFormula = dbConn.PowerQueryFormula;

                    if (powerQueryFormula != null)
                    {
                        // Visa egenskaperna för PowerQueryFormula.
                        Console.WriteLine("PowerQueryFormula Type: " + powerQueryFormula.Type);
                        Console.WriteLine("PowerQueryFormula GroupName: " + powerQueryFormula.GroupName);
                        Console.WriteLine("PowerQueryFormula FormulaDefinition: " + powerQueryFormula.FormulaDefinition);
                        Console.WriteLine("PowerQueryFormula Name: " + powerQueryFormula.Name);
                        Console.WriteLine("PowerQueryFormula Description: " + powerQueryFormula.Description);

                        // Demonstrera åtkomst till samlingen PowerQueryFormulaItems.
                        Console.WriteLine("Number of PowerQueryFormulaItems: " + powerQueryFormula.PowerQueryFormulaItems.Count);
                    }
                    else
                    {
                        Console.WriteLine("PowerQueryFormula is null for this connection.");
                    }
                }

                // Spara arbetsboken
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

### Se även

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


