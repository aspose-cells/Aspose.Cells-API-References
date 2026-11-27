---
title: "WebExtensionProperty.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionProperty-egenskap. Hämtar och anger ett anpassat egenskapsvärde"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Hämtar och sätter ett anpassat egenskapsvärde.

```csharp
public string Value { get; set; }
```

### Exempel

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
                // Skapa en WebExtensionProperty-instans
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Ställ in och demonstrera Value-egenskapen
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Ändra och visa uppdaterat värde
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

### Se även

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


