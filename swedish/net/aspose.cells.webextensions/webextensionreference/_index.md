---
title: "Klass WebExtensionReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionReference-klass. Representerar identifiering av leverantörens plats och version av tillägget"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Representerar identifiering av leverantörens plats och version av tillägget.

```csharp
public class WebExtensionReference
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Hämtar och anger identifieraren som är associerad med Office-tillägget inom en katalogleverantör. Identifieraren MÅSTE vara unik inom en katalogleverantör. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Hämtar och anger instansen av marknadsplatsen där Office-tillägget lagras. . |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Hämtar och anger typen av marknadsplats som lagrattributet identifierar. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Hämtar och anger versionen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en WebExtension först
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Hämta WebExtensionReference från WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Ställ in egenskaper för WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Visa referensegenskaper
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Spara arbetsboken
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


