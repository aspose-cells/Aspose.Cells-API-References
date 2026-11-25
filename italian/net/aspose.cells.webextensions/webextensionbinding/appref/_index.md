---
title: "WebExtensionBinding.Appref"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionBinding. Ottiene e imposta la chiave di binding usata per mappare la voce di binding in questo elenco con i dati collegati nel documento"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Ottiene e imposta la chiave di binding utilizzata per mappare la voce di binding in questo elenco con i dati collegati nel documento.

```csharp
public string Appref { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyApprefDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Imposta le proprietà includendo Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Visualizza il valore corrente di Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Modifica il valore di Appref per dimostrare che è leggibile/scrivibile
                binding.Appref = "Sheet1!C3:D4";
                Console.WriteLine("Updated Appref value: " + binding.Appref);
                
                Console.WriteLine("Appref property has been successfully demonstrated");
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


