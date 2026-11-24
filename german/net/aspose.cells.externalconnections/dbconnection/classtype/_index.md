---
title: "DBConnection.ClassType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection‑Eigenschaft. Gibt den Typ dieses ExternalConnection‑Objekts zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

Gibt den Typ dieses [`ExternalConnection`](../../externalconnection/) Objekts zurück.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine neue DBConnection‑Instanz, indem du sie zur Sammlung hinzufügst
                // Da DBConnection keinen öffentlichen parameterlosen Konstruktor hat,
                // lassen wir die Sammlung ihn für uns erstellen
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Anzeige des ClassType-Werts (schreibgeschützte Eigenschaft)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Demonstration des Setzens anderer Eigenschaften, um das Beispiel aussagekräftiger zu machen
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Speichere die Arbeitsmappe
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


