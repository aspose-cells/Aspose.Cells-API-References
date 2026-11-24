---
title: "WebQueryConnection.IsParsePre"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Kennzeichen, das angibt, ob Daten, die in HTML-PRE-Tags auf der Webseite enthalten sind, beim Importieren der Seite in eine Abfragetabelle in Spalten geparst werden."
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Flag, das angibt, ob Daten, die in HTML‑PRE‑Tags auf der Webseite enthalten sind, beim Importieren der Seite in eine Abfragetabelle in Spalten aufgeteilt werden.

```csharp
public bool IsParsePre { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine neue Webabfrageverbindung unter Verwendung der vorhandenen Verbindung aus der Arbeitsmappe
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Zeige den anfänglichen IsParsePre-Wert an (Standard)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Setze IsParsePre auf true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Setze IsParsePre zurück auf false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Speichere die Arbeitsmappe
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


