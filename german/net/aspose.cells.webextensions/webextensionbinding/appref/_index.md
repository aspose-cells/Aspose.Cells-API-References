---
title: "WebExtensionBinding.Appref"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionBinding-Eigenschaft. Gibt den Bindungsschlüssel zurück und setzt ihn, der verwendet wird, um den Bindungseintrag in dieser Liste mit den gebundenen Daten im Dokument zu verknüpfen"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Liefert und setzt den Bindungsschlüssel, der verwendet wird, um den Bindungseintrag in dieser Liste mit den gebundenen Daten im Dokument zu verknüpfen.

```csharp
public string Appref { get; set; }
```

### Beispiele

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
                // Erstelle eine neue WebExtensionBinding-Instanz
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Setzen Sie Eigenschaften einschließlich Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Den aktuellen Wert von Appref anzeigen
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Den Appref-Wert ändern, um zu demonstrieren, dass er les- und schreibbar ist
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

### Siehe auch

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


