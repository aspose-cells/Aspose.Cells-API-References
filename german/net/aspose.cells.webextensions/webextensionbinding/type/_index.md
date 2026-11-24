---
title: "WebExtensionBinding.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionBinding-Eigenschaft. Gibt den Bindungstyp zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Liest und setzt den Bindungstyp.

```csharp
public string Type { get; set; }
```

### Beispiele

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
                // Erstelle eine neue WebExtensionBinding-Instanz
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Setze die Type-Eigenschaft
                binding.Type = "text";
                
                // Den aktuellen Wert von Type anzeigen
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Den Type-Wert ändern, um zu demonstrieren, dass er les- und schreibbar ist
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

### Siehe auch

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


