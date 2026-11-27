---
title: "Klass WebExtensionBinding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionBinding class. Representerar ett bindningsförhållande mellan ett Office-tillägg och data i dokumentet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Representerar ett bindningsförhållande mellan ett Office-tillägg och data i dokumentet.

```csharp
public class WebExtensionBinding
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Hämtar och anger bindningsnyckeln som används för att mappa bindningsposten i den här listan med de bundna data i dokumentet. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Hämtar och anger bindningsidentifieraren. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Hämtar och anger bindningstypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny WebExtensionBinding-instans
                WebExtensionBinding binding = new WebExtensionBinding();

                // Ställ in egenskaper
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Visa egenskapsvärden
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Ändra egenskaper
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


