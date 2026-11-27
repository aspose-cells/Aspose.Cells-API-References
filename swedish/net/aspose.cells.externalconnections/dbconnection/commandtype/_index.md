---
title: "DBConnection.CommandType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection‑egenskap. Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webb‑baserad List Data Provider"
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webbaserad List Data Provider.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Initiera en arbetsbok (tom eller från en fil som kan innehålla anslutningar)
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
                    // Visa det aktuella CommandType‑värdet
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Demonstrera att sätta CommandType (läslig‑skrivbar egenskap)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Spara arbetsboken (även om den är oförändrad) för att illustrera ett komplett flöde
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


