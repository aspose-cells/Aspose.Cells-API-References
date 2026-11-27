---
title: "WebExtensionBinding.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionBinding‑egenskap. Hämtar och anger bindningstypen"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Hämtar och anger bindningstypen.

```csharp
public string Type { get; set; }
```

### Exempel

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
                // Skapa en ny WebExtensionBinding-instans
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Ange Type‑egenskapen
                binding.Type = "text";
                
                // Visa det aktuella värdet för Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Ändra Type‑värdet för att demonstrera att det är läs/skriv
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

### Se även

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


