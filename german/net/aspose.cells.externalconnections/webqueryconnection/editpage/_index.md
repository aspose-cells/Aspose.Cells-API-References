---
title: "WebQueryConnection.EditPage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird beibehalten, falls sourceDatatrue und url auf eine XML-Datei umgeleitet wurden. Dann kann die benutzerorientierte Seite in der UI angezeigt und die XML-Daten im Hintergrund abgerufen werden."
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden und die XML-Daten können im Hintergrund abgerufen werden.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft WebQueryConnection.EditWebPage. Diese Eigenschaft wird 12 Monate später, seit Oktober 2017, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste vorhandene Webabfrageverbindung zu, falls verfügbar
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Anzeigen des anfänglichen EditPage-Werts
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Setzen Sie EditPage auf eine neue URL (da es les‑ und schreibbar ist)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Speichere die Arbeitsmappe
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


