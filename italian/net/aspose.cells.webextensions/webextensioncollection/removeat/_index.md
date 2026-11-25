---
title: "WebExtensionCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebExtensionCollection. Rimuove l'estensione web per indice"
type: docs
url: /it/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Rimuovi l'estensione web per indice.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una collezione di estensioni web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Aggiungi alcune estensioni web alla raccolta
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Chiama il metodo RemoveAt con parametro Int32
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


