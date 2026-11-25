---
title: "WebExtensionReferenceCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionReferenceCollection. Ottiene l'estensione web per l'indice specifico"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Ottiene l'estensione web per l'indice specifico.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

L'estensione web

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Aggiunge un nuovo riferimento dell'estensione web
                int index = references.Add();
                
                // Accedi alla proprietà Item (di sola lettura) per ottenere il riferimento all'indice specificato
                WebExtensionReference reference = references[index];
                
                // Visualizza le informazioni sul riferimento recuperato
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Nota: La proprietà Item è di sola lettura, quindi dimostriamo solo il recupero del suo valore
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


