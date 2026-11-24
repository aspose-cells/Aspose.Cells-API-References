---
title: "WebQueryConnection.IsXl2000"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection-Eigenschaft. Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und wird auf true gesetzt, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung, die neuer oder gleich Microsoft Excel 2000 ist, aktualisiert wurde. Dies ist ein optionales Attribut, das ignoriert werden kann"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung, die neuer oder gleich Microsoft Excel 2000 ist, aktualisiert wurde. Dies ist ein optionales Attribut, das ignoriert werden kann.

```csharp
public bool IsXl2000 { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
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
                    // Zeige den anfänglichen IsXl2000-Wert an
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Setze IsXl2000 auf true (da es les- und schreibbar ist)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Setze IsXl2000 zurück auf false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Speichere die Arbeitsmappe
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
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


