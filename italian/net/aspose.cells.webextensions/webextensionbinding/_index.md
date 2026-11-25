---
title: "Classe WebExtensionBinding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionBinding. Rappresenta una relazione di binding tra un Office Addin e i dati nel documento"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Rappresenta una relazione di binding tra un Office Add-in e i dati nel documento.

```csharp
public class WebExtensionBinding
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Ottiene e imposta la chiave di binding utilizzata per mappare la voce di binding in questo elenco con i dati collegati nel documento. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Ottiene e imposta l'identificatore di binding. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Ottiene e imposta il tipo di binding. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();

                // Imposta le proprietà
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Visualizza i valori delle proprietà
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Modifica proprietà
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


