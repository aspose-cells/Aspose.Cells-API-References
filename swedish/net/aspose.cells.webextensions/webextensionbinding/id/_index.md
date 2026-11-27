---
title: "WebExtensionBinding.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionBinding‑egenskap. Hämtar och anger bindningsidentifieraren"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Hämtar och anger bindningsidentifieraren.

```csharp
public string Id { get; set; }
```

### Exempel

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
                // Skapa en ny WebExtensionBinding-instans
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Ange Id‑egenskapen
                binding.Id = "SampleBindingId";
                
                // Visa det aktuella värdet för Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Ändra Id‑värdet för att demonstrera att det är läs/skriv
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

### Se även

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


