---
title: "WebExtensionBinding.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionBinding. Ottiene e imposta il tipo di binding"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Ottiene e imposta il tipo di binding.

```csharp
public string Type { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Imposta la proprietà Type
                binding.Type = "text";
                
                // Visualizza il valore corrente di Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Modifica il valore di Type per dimostrare che è leggibile/scrivibile
                binding.Type = "range";
                Console.WriteLine("Updated Type value: " + binding.Type);
                
                Console.WriteLine("Type property has been successfully demonstrated");
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


