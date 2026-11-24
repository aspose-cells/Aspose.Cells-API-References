---
title: "WebExtensionProperty.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionProperty-Eigenschaft. Gibt einen benutzerdefinierten Eigenschaftswert zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Liest und setzt einen benutzerdefinierten Eigenschaftswert.

```csharp
public string Value { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Eine WebExtensionProperty-Instanz erstellen
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Value-Eigenschaft festlegen und demonstrieren
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Wert ändern und aktualisierten Wert anzeigen
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


