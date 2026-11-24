---
title: "Klasse WebExtensionProperty"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionProperty Klasse. Stellt eine benutzerdefinierte Eigenschaft eines Office‑Add‑Ins dar"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Stellt eine benutzerdefinierte Eigenschaft eines Office-Add-Ins dar.

```csharp
public class WebExtensionProperty
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Liest und setzt einen benutzerdefinierten Eigenschaftsnamen. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Liest und setzt einen benutzerdefinierten Eigenschaftswert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine neue Instanz von WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Setze Eigenschaftswerte
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Zeige die Eigenschaftswerte an
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


