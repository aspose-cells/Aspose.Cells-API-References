---
title: "ExternalConnection.SSOId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Kennung für Single Sign On (SSO), die für die Authentifizierung zwischen einem Zwischenspeicher‑SpreadsheetML‑Server und der externen Datenquelle verwendet wird"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Bezeichner für Single Sign On (SSO), das für die Authentifizierung zwischen einem Zwischenserver für spreadsheetML und der externen Datenquelle verwendet wird.

```csharp
public string SSOId { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeigen Sie den anfänglichen SSOId-Wert an (wahrscheinlich null für neue Verbindungen)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Setzen Sie einen neuen SSOId-Wert (da er les- und schreibbar ist)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Löschen Sie die SSOId
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
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

### Siehe auch

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


