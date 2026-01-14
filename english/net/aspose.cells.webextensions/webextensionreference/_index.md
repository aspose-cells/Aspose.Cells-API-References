---
title: Class WebExtensionReference
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WebExtensions.WebExtensionReference class. Represents identify the provider location and version of the extension
type: docs
url: /net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Represents identify the provider location and version of the extension.

```csharp
public class WebExtensionReference
```

## Properties

| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Gets and sets the type of marketplace that the store attribute identifies. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Gets and sets the version. |

### Examples

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
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a WebExtension first
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Get the WebExtensionReference from the WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Set properties of the WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Display the reference properties
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Save the workbook
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

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


