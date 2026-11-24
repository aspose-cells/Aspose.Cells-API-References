---
title: "WebQueryConnection.EditWebPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird beibehalten, falls sourceDatatrue und url auf eine XML-Datei umgeleitet wurden. Dann kann die benutzerorientierte Seite in der UI angezeigt und die XML-Daten im Hintergrund abgerufen werden."
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden und die XML-Daten können im Hintergrund abgerufen werden.

```csharp
public string EditWebPage { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf die erste vorhandene WebQueryConnection zu (falls vorhanden)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Setzen Sie den anfänglichen EditWebPage-Wert
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Aktualisieren Sie den EditWebPage-Wert
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Speichere die Arbeitsmappe mit der WebQueryConnection
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


