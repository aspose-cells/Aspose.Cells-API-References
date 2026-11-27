---
title: "DBConnection.ConnectionInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection‑egenskap. Strängen med anslutningsinformation används för att kontakta en OLE DB‑ eller ODBC‑datakälla"
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ExternalConnection.ConnectionString‑egenskapen. Denna metod kommer att tas bort 12 månader senare, från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionInfoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Skapa en ny DBConnection‑instans genom att lägga till den i samlingen
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Ställ in en grundläggande anslutning för att demonstrera ConnectionInfo‑egenskapen
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Visa det aktuella värdet för ConnectionInfo‑egenskapen
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Eftersom ConnectionInfo inte är skrivskyddad, demonstrera hur man sätter den
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Spara arbetsboken
                workbook.Save("ConnectionInfoDemo.xlsx");

                Console.WriteLine("ConnectionInfo demonstration completed successfully.");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


