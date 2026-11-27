---
title: "WebExtensionBinding.Appref"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionBinding egenskap. Hämtar och anger bindningsnyckeln som används för att mappa bindningsposten i den här listan med de bundna data i dokumentet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Hämtar och anger bindningsnyckeln som används för att mappa bindningsposten i den här listan med de bundna data i dokumentet.

```csharp
public string Appref { get; set; }
```

### Exempel

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
                // Skapa en ny WebExtensionBinding-instans
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Ställ in egenskaper inklusive Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Visa det aktuella värdet för Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Ändra Appref‑värdet för att demonstrera att det är läs/skriv
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

### Se även

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


