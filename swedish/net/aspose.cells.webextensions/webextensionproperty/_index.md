---
title: "Klass WebExtensionProperty"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionProperty-klass. Representerar en anpassad egenskap för Office‑tillägg"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Representerar en anpassad egenskap för ett Office-tillägg.

```csharp
public class WebExtensionProperty
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Hämtar och sätter ett anpassat egenskapsnamn. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Hämtar och sätter ett anpassat egenskapsvärde. |

### Exempel

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
                // Skapa en ny instans av WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Ställ in egenskapsvärden
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Visa egenskapsvärdena
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

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


