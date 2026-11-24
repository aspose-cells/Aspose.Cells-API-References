---
title: "DBConnection.CommandType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection-Eigenschaft. Gibt den OLE DB-Befehlstyp an. 1. Abfrage gibt einen Würfelnamen an 2. Abfrage gibt eine SQL-Anweisung an 3. Abfrage gibt einen Tabellennamen an 4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden und es dem Anbieter überlassen ist, wie diese zu interpretieren sind. 5. Abfrage erfolgt gegen einen webbasierten List Data Provider"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Gibt den OLE DB-Befehlstyp an. 1. Abfrage gibt einen Würfelnamen an 2. Abfrage gibt eine SQL-Anweisung an 3. Abfrage gibt einen Tabellennamen an 4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese interpretiert werden. 5. Abfrage erfolgt gegen einen webbasierten List Data Provider.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Beispiele

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
            // Initialisieren Sie eine Arbeitsmappe (leer oder aus einer Datei, die Verbindungen enthalten kann)
            Workbook workbook = new Workbook();

            try
            {
                // Zugriff auf die Sammlung externer Verbindungen
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Finde die erste DBConnection in der Sammlung (falls vorhanden)
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
                    // Zeigen Sie den aktuellen CommandType-Wert an
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Demonstrieren Sie das Setzen von CommandType (Lese‑/Schreib‑Eigenschaft)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Speichern Sie die Arbeitsmappe (auch wenn unverändert), um einen vollständigen Ablauf zu veranschaulichen
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

### Siehe auch

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


