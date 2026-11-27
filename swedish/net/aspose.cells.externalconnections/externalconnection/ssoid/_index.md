---
title: "ExternalConnection.SSOId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML-server och den externa datakällan"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan.

```csharp
public string SSOId { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det ursprungliga SSOId‑värdet (troligen null för ny anslutning)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Ange ett nytt SSOId‑värde (eftersom det är läs‑skriv)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Rensa SSOId‑värdet
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("SSOIdDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


