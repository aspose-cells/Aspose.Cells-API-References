---
title: "WebExtensionProperty.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionProperty-egenskap. Hämtar och anger ett anpassat egenskapsnamn"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Hämtar och sätter ett anpassat egenskapsnamn.

```csharp
public string Name { get; set; }
```

### Exempel

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
                // Skapa en WebExtensionProperty-instans
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Ställ in och demonstrera Name-egenskapen
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Ändra och visa uppdaterat namn
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

### Se även

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


