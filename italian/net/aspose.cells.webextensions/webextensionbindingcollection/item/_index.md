---
title: "WebExtensionBindingCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionBindingCollection. Ottiene la relazione di binding dell'estensione web per l'indice specifico"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Ottiene la relazione di binding della web extension per l'indice specifico.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La relazione di binding dell'estensione web

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una collezione di binding dell'estensione web
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Aggiungi un nuovo binding alla collezione
            int index = bindingCollection.Add();

            // Accedi al binding usando la proprietà Item (sola lettura)
            WebExtensionBinding binding = bindingCollection[index];

            // Imposta le proprietà sul binding
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Visualizza i dettagli del binding
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Modifica il binding attraverso la collezione
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Salva la cartella di lavoro
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


