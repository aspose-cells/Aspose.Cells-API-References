---
title: "WebExtensionBinding.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionBinding. Ottiene e imposta l'identificatore del binding"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Ottiene e imposta l'identificatore di binding.

```csharp
public string Id { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyIdDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Imposta la proprietà Id
                binding.Id = "SampleBindingId";
                
                // Visualizza il valore corrente di Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Modifica il valore di Id per dimostrare che è leggibile/scrivibile
                binding.Id = "UpdatedBindingId";
                Console.WriteLine("Updated Id value: " + binding.Id);
                
                Console.WriteLine("Id property has been successfully demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


