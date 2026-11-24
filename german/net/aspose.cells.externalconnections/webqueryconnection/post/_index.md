---
title: "WebQueryConnection.Post"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Gibt die Zeichenkette zurück oder setzt sie, die mit der POST-Methode verwendet wird, um Daten an einen Webserver zu senden und Daten aus einer Webabfrage zurückzuerhalten."
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Gibt die Zeichenfolge zurück oder legt sie fest, die mit der POST‑Methode zum Senden von Daten an einen Webserver verwendet wird, um Daten aus einer Webabfrage zurückzugeben.

```csharp
public string Post { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine Webabfrageverbindung, indem du eine vorhandene nutzt oder sie durch korrekte Initialisierung erstellst
                // Da wir WebQueryConnection nicht direkt instanziieren können, verwenden wir die erste Verbindung, falls sie existiert
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Falls keine Verbindungen existieren, demonstrieren wir mit einer Mock-Verbindung
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Setze den anfänglichen Post-Wert
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Ändere den Post-Wert
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Löschen Sie den Post-Wert
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Speichere die Arbeitsmappe
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


