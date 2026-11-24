---
title: "WebQueryConnection.ClassType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Gibt den Typ dieses ExternalConnection-Objekts zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

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

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf eine vorhandene Webabfrageverbindung zu oder erstelle eine über die richtige Initialisierung
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Anzeige des ClassType-Werts (schreibgeschützte Eigenschaft)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Überprüfen Sie den erwarteten Enum-Wert für die Webabfrage
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Speichere die Arbeitsmappe
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


