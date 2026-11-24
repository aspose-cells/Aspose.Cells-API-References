---
title: "WebExtensionBinding.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionBinding-Eigenschaft. Gibt den Bindungsbezeichner zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Liefert und setzt den Bindungsbezeichner.

```csharp
public string Id { get; set; }
```

### Beispiele

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
                // Erstelle eine neue WebExtensionBinding-Instanz
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Setze die Id-Eigenschaft
                binding.Id = "SampleBindingId";
                
                // Den aktuellen Wert von Id anzeigen
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Den Id-Wert ändern, um zu demonstrieren, dass er les- und schreibbar ist
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

### Siehe auch

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


