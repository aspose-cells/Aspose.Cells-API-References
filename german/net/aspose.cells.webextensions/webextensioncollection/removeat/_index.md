---
title: "WebExtensionCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionCollection-Methode. Entfernt die Web-Extension nach Index"
type: docs
url: /de/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Web-Extension nach Index entfernen.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Web-Extension-Sammlung erstellen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Fügen Sie einige Web-Erweiterungen zur Sammlung hinzu
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Rufen Sie die RemoveAt-Methode mit dem Int32-Parameter auf
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


