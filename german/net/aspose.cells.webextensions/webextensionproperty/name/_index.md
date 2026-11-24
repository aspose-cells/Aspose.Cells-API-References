---
title: "WebExtensionProperty.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionProperty-Eigenschaft. Gibt einen benutzerdefinierten Eigenschaftsnamen zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Liest und setzt einen benutzerdefinierten Eigenschaftsnamen.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Eine WebExtensionProperty-Instanz erstellen
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Name-Eigenschaft festlegen und demonstrieren
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Namen ändern und aktualisierten Namen anzeigen
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
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


