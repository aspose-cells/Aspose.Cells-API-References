---
title: "DataModelConnection.ConnectionString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelConnection‑egenskap. Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla"
type: docs
url: /sv/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla.

```csharp
public override string ConnectionString { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en DataModelConnection‑instans med ett oinitierat objekt
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Visa initialt ConnectionString‑värde (tomt)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Ställ in ConnectionString‑egenskapen
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Visa det uppdaterade ConnectionString‑värdet
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Ställ in andra nödvändiga egenskaper för en fullständig anslutning
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Spara arbetsboken med anslutningen
                workbook.Save("ConnectionStringDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


