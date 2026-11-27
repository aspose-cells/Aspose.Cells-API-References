---
title: "WebExtensionCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionCollection‑metod. Tar bort webbutökning med indexet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Ta bort webbutökning med indexet.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en samling av webbutökningar
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Lägg till några webbtillägg i samlingen
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Anropa RemoveAt-metoden med Int32-parameter
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


